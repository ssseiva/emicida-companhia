# Emicida e companhia — cronograma

Cronograma de produção do clube de leitura, parceria entre **Seiva**, **Companhia das Letras** e **Emicida**.
Documento complementar ao deck de conceito.

Período coberto: 16 de agosto a 5 de dezembro de 2026.

## O que tem aqui

`index.html` — página única, sem dependências externas. As fontes (Neue Haas Display e
Editorial New) estão embutidas como woff2 em base64, então o arquivo abre em qualquer
navegador, offline inclusive.

- Calendário completo, dia a dia, com código de cores por tipo de peça
- Filtros por trilha: produção interna, marketing e entregas para inscritos
- Detalhe de cada item no hover
- Inventário de entregas contado a partir do próprio calendário
- Pontos que ainda precisam de decisão

`Ctrl+P` gera um PDF em A4 deitado, com o layout forçado para fundo claro.

## Editando

Todo o conteúdo do calendário vive em duas listas no `<script>` no fim do arquivo:

- `EV` — itens de um dia só
- `PERIODS` — tarefas contínuas, que se cortam sozinhas nas semanas

O calendário, o inventário e a lista do Emicida são todos gerados a partir dessas listas,
então os números nunca divergem do desenho.
