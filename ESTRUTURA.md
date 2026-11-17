# Estrutura do código

Tudo vive em `index.html`, um arquivo de cerca de 2 MB, sem build. Ele é montado por um script que junta o CSS, a arte, os dados e a aplicação. Editar direto no `index.html` funciona, mas os dados ficam num bloco JSON grande; para mudanças de conteúdo, prefira o card **Importar / Exportar**.

---

## Mapa do arquivo

| Bloco | Conteúdo |
| --- | --- |
| `<style id="app-css">` | Tema: parede verde, papel, dourado, o azul de Rosália |
| `<script id="seed-img">` | Retratos de reserva (vazio nesta cópia) |
| `<script id="state">` | Todo o conteúdo: série, episódios, roteiros, personagens, glossário, aulas, histórico |
| Arte (`D`) | Desenhos em SVG gerados em código (cenários, storyboard, ícones) |
| Aplicação | Store, campos com histórico, roteador, renderizadores, importação, exportação |

---

## Persistência

Escolhida em tempo de carga:

```js
artefato do Claude   // dentro do Claude: a página se republica com o estado novo
localStorage         // navegador comum, chave "ppdmd-state"
```

Fora do Claude, a primeira carga usa o estado embutido; depois de uma edição, o navegador passa a usar a cópia salva em `localStorage`. **Importar / Exportar** gera um JSON com os dados e um HTML autônomo com tudo.

---

## O estado

```js
{
  series: { blocks: { logline:{type,v}, sinopse:{...}, roteiros:{...}, ... } },
  eps: [ { n, titulo, teaser, resumo, argumento:[cenas], roteiro:[cenas],
           papeis, perguntas, furos, diffs, melhorias, sugestao, sb } ],
  chars: [ { id, nome, f:{ficha}, psico, traj:[[ep, texto]], duvidas } ],
  gloss, aulas, diretor, notas,
  img:  { id: dataURL },          // retratos
  hist: { caminho: [versões] },   // repositório histórico
  upd:  { caminho: {ts, src} },   // última atualização de cada campo
  log:  [ alterações ]
}
```

Cada campo tem um caminho, como `ep.4.resumo`, `series.riscos` ou `char.ana.traj`. Quando um campo muda, a versão anterior entra no topo de `hist[caminho]` com data e origem.

---

## Roteador

Por hash: `#serie`, `#ep-7`, `#personagens`, `#p-ana`, `#glossario`, `#storyboard`, `#diretor`, `#roteirizando`, `#importar`, `#dados`. Cada rota chama uma função `v…()` que devolve o HTML da tela.

---

## Arte

Nenhuma imagem de cena vem da rede. Cenários e painéis de storyboard são SVG gerados em código; os retratos dos personagens estão embutidos como imagens.
