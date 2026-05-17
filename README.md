# Brainiac

Brainiac e um app para organizar uma liguinha de Magic: The Gathering no formato Commander multiplayer, substituindo processos hoje manuais como inscricao em eventos, montagem de mesas, validacao de resultados e consolidacao de rankings.

## Objetivo do primeiro teste

Validar se um painel web simples consegue substituir, com confianca, os fluxos mais trabalhosos do dia a dia da liguinha:

1. inscricao no evento;
2. organizacao das mesas por rodada;
3. registro e validacao de resultados;
4. ranking do dia;
5. ranking geral da season.

## Escopo inicial

- seasons com duracao aproximada de 6 meses;
- calendario de eventos tematicos;
- inscricao por evento com confirmacao de presenca, pedido da Vault, pagamento e deck submetido;
- validacao manual dos decks pelo conselho;
- 4 rodadas por evento;
- pods preferencialmente com 4 jogadores, aceitando mesas de 3 quando necessario;
- geracao da rodada 1 a partir do ranking geral da season;
- geracao das rodadas seguintes a partir do ranking parcial do dia;
- validacao de resultados pelo conselho antes de a rodada seguinte ser montada;
- leaderboard do dia e leaderboard geral da season.

## Documentacao inicial

- [Visao do produto](docs/product-brief.md)
- [Regras de negocio](docs/rules.md)
- [Modelo de dominio](docs/domain-model.md)
- [Backlog inicial](docs/backlog.md)
- [Decisoes em aberto](docs/open-decisions.md)

## Principios do MVP

- resolver primeiro o trabalho do organizador e do conselho;
- manter o ranking derivado de resultados validados;
- preferir validacao manual onde a automacao ainda nao estiver provada;
- deixar login de jogadores e tracking detalhado de partida para fases posteriores.
