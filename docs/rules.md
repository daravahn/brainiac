# Regras de negocio

## Estrutura geral

- Uma season dura aproximadamente 6 meses.
- Uma season possui varios eventos.
- Cada evento possui 4 rodadas.
- O formato e Commander multiplayer, cada jogador por si.
- Os pods devem ter preferencialmente 4 jogadores.
- Quando o numero de participantes nao permitir apenas pods de 4, podem existir pods de 3.

## Inscricao no evento

Cada jogador inscrito em um evento deve informar:

- confirmacao de presenca;
- pedido da Vault;
- status de pagamento da taxa de participacao de R$ 20;
- link do deck que pretende usar;
- deck submetido para conferencia de budget.

O torneio e budget, com limite de R$ 100 incluindo o commander.

## Formacao das mesas

- Na rodada 1, os jogadores sao ordenados pelo ranking geral da season.
- A distribuicao acontece a partir dessa ordem para formar os pods da rodada.
- Da rodada 2 em diante, a ordenacao usa o ranking parcial do proprio evento.
- O sistema deve considerar apenas resultados validados para gerar a rodada seguinte.

## Pontuacao padrao

- 1o lugar da mesa: 3 pontos;
- 2o lugar da mesa: 2 pontos;
- demais jogadores: 1 ponto.

## Empates

- Em caso de empate, os jogadores ainda vivos recebem 1 ponto.
- Jogadores eliminados antes do empate nao recebem o ponto de empate.

## Dia de troca de decks

- Existe pelo menos uma regra especial ja conhecida: quando o deck de um jogador termina em 1o lugar, esse jogador recebe 1 ponto extra.
- A modelagem final dessa regra ainda depende de confirmar se o bonus pertence ao dono original do deck ou ao piloto do deck naquela partida.

## Validacao

- Resultados de mesa precisam ser validados por um membro do conselho.
- Apenas resultados validados entram nos calculos oficiais de ranking e no pareamento da rodada seguinte.

## Rankings

O sistema deve manter duas visoes:

- ranking do evento, recalculado a cada rodada;
- ranking geral da season, acumulado entre eventos.
