# Arquitetura inicial

## Direcao

O projeto seguira com frontend Flutter para web, Android e iOS desde o inicio, mantendo web e mobile como superficies de primeira classe.

## Componentes

- Flutter app
  - experiencia do jogador em mobile;
  - experiencia administrativa responsiva para web;
- ASP.NET Core API
  - autenticacao;
  - regras de dominio;
  - endpoints para seasons, eventos, jogadores, rodadas, pods e rankings;
- banco relacional
  - persistencia transacional das entidades de torneio.

## Backend minimo viavel

O primeiro backend pode nascer com:

- players;
- papeis de acesso:
  - player;
  - admin_conselho;
  - admin_geral;
- seasons;
- events;
- wizard event code;
- rounds;
- pods;
- pod players;
- resultados;
- standings derivados.

## Autenticacao

Direcao inicial:

- login Google para equipe administrativa e, se a experiencia justificar, tambem para jogadores;
- autorizacao por role no backend;
- formulario publico ainda pode existir no primeiro piloto se reduzir atrito para jogadores.

## Persistencia

Direcao inicial:

- banco relacional;
- migrations versionadas;
- standings calculados a partir de resultados validados;
- evitar tabelas duplicadas de ranking como fonte primaria de verdade.

## Separacao de superficies

- mobile-first para experiencia do jogador;
- web responsiva e densa para organizador e conselho;
- mesma regra de negocio e mesmo backend para todas as plataformas;
- composicao visual adaptada por superficie, em vez de copiar literalmente a mesma tela para todo lugar.
