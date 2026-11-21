# Pra eu parar de me doer · Sala de Roteiro

Plataforma de desenvolvimento da série limitada **Pra eu parar de me doer**: drama espiritual e suspense sobrenatural brasileiro, 12 capítulos.

**[▶ Abrir a sala de roteiro](https://zanitchy.github.io/pra-eu-parar-de-me-doer/)**

João aluga um casarão antigo e, na parede da sala, encontra o retrato de Rosália, uma mulher morta no início do século XIX. Ela sai da tela, faz um pacto com ele e o obriga a trazer de volta o homem que a matou. A cada capítulo, João desconfia de alguém diferente: a esposa, a vizinha, a neta da vizinha, a ex-mulher do dono da casa. A outra metade de Rosália estava ao lado dele desde o começo.

Série, episódios, personagens, roteiros, escaletas e a leitura crítica de cada capítulo ficam em **uma página só**, sem build, sem instalação e sem servidor. Abre offline com duplo clique.

Roteiro de **Roberto Pazzini**.

---

## Os cards

| Card | O que é |
| --- | --- |
| **Série** | Logline, sinopse, premissa, ideia controladora, temas, tom, referências, linguagem visual, estrutura (Jornada do Herói e McKee), cenários, os 12 argumentos, a leitura dos roteiros, riscos, perguntas estratégicas, inconsistências e sugestões para a escaleta, cada item com a cena e a página onde aparece |
| **Episódios** | Os 12 capítulos: título, teaser, resumo, escaleta cena a cena, roteiro completo, papéis dos personagens, perguntas do especialista, furos do roteiro, diferenças entre escaleta e roteiro, melhorias e sugestão, cada item com a cena e a página do roteiro e a cena da escaleta |
| **Personagens** | Fichas com retrato, perfil completo, leitura psicológica, trajetória episódio a episódio e dúvidas |
| **Glossário** | Termos de roteiro, cada um exemplificado dentro da própria série |
| **Dúvidas do especialista** | As 216 perguntas do especialista (série, episódios e personagens) num lugar só, cada uma com a situação no roteiro, onde aparece, o espaço para a resposta do autor e o histórico. Dentro do Claude, reavalia as dúvidas depois de mudanças no roteiro e levanta dúvidas novas |
| **Storyboard** | Um painel por cena (256 no total), com a ação, o plano e o movimento, o porquê da escolha, luz e som, a transição e a localização no roteiro e na escaleta |
| **Pergunte ao Diretor** | Perguntas e respostas sobre a série (só dentro do Claude) |
| **Roteirizando** | Aula de roteiro com professor (só dentro do Claude) |
| **Arquivos** | Importa roteiros e escaletas para atualizar os cards |
| **Importar / Exportar** | Backup dos dados e do HTML |

---

## Os 12 capítulos

| # | Título | Páginas do roteiro |
| --- | --- | --- |
| 01 | O Retrato | 38 |
| 02 | Febre | 58 |
| 03 | O Pacto | 65 |
| 04 | Berço Vazio | 83 |
| 05 | Quem é Quem | 82 |
| 06 | Semelhanças | 74 |
| 07 | Chopin para Ninguém | 69 |
| 08 | O Fim Está Próximo | 55 |
| 09 | A Essência | 53 |
| 10 | Fumaça Branca | 53 |
| 11 | O Jantar | 48 |
| 12 | Pra Eu Parar de Me Doer | 33 |

---

## A leitura crítica

Cada capítulo foi lido como roteiro de produção: o que funciona, o que contradiz o resto da série, o que mudou da escaleta para o roteiro e o que cortar. O card **Série** reúne a visão de conjunto. Os quatro pontos que pedem decisão antes da próxima versão:

1. **A relação entre Ana e Giuseppe.** O capítulo 11 revela que começou quando ele tinha 16 anos, e o roteiro a chama de “amantes”. Ninguém em cena nomeia o que foi.
2. **O final escolhe a vingança.** Rosália mata Giuseppe e sobe à luz; ele pede perdão e é arrastado por sombras. Isso contradiz o discurso do perdão (cap. 3) e a narração espírita do epílogo.
3. **João sai sem culpa.** Ele aceita que Giuseppe tem de morrer (cap. 10) e o deixa no fogo (cap. 12).
4. **Pistas sem resposta.** Tomé e a tiara, a mãe de Ana parecida com Rosália, o plano de Iara, os sinais de Beatriz.

Somam-se os nós de continuidade: século XVIII × XIX, Itália × Espanha, ritual × apego, Ana e Iara amigas ou desconhecidas, a idade dos personagens no epílogo.

---

## Repositório histórico

Todo campo editável guarda a versão anterior. Ao alterar um resumo, uma ficha ou uma nota (na mão ou por importação de arquivo), o texto antigo desce para o histórico do campo, com data, hora e a origem da mudança. Nada é sobrescrito em silêncio.

---

## Dentro e fora do Claude

A plataforma nasceu como artefato do Claude e roda nos dois lugares:

| | Dentro do Claude | Fora (navegador) |
| --- | --- | --- |
| Cards, roteiros, históricos, glossário, storyboard | ✅ | ✅ |
| Edição de campos | ✅ salva no artefato | ✅ salva no navegador (`localStorage`) |
| Importação de roteiros e escaletas | ✅ | ✅ só o reconhecimento automático |
| Pergunte ao Diretor · Roteirizando · leitura crítica por IA | ✅ | ❌ consulta das respostas já salvas |

Nesta cópia, os recursos de IA mostram um aviso em vez de falhar em silêncio. As edições feitas aqui ficam só no seu navegador; para levá-las adiante, use **Importar / Exportar**.

Esta cópia é uma fotografia do artefato em 17/11/2026 e só é atualizada quando pedido.

---

## Estrutura

Arquivo único, sem dependências de build. As fontes vêm do Google Fonts; o resto (retratos, arte em SVG, dados) está embutido.

```
index.html      a plataforma inteira (aplicação + dados)
README.md       este arquivo
ESTRUTURA.md    mapa do código
LICENSE         MIT (código)
.nojekyll       serve o arquivo cru no Pages
```

Detalhes em [ESTRUTURA.md](ESTRUTURA.md).

---

## Números

| | |
| --- | --- |
| Capítulos | 12 |
| Cenas nos roteiros | 256 |
| Cenas nas escaletas | 232 |
| Páginas de roteiro | 711 |
| Personagens fichados | 25 |
| Furos e inconsistências registrados nos capítulos | 94 |
| Melhorias sugeridas | 57 |
| Painéis de storyboard | 256 (um por cena) |
| Dúvidas do especialista | 216 (48 respondidas, 168 pendentes na leitura inicial) |
| Termos no glossário | 57 |
| Texto dos roteiros embutido | ~520 mil caracteres |

---

## Licença

O **código** está sob MIT. A **série** (roteiros, escaletas, argumentos, personagens e todo o material narrativo) pertence ao seu autor e não está licenciada para uso, adaptação ou produção.
