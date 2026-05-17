# ADR 0003: Codigo da Wizard no evento

## Status

Aceita

## Contexto

Os jogadores ja precisam inserir um codigo no app da Wizard no dia do evento.

## Decisao

Registrar o codigo da Wizard no `Event` e disponibiliza-lo para copia no app em uma janela proxima ao inicio do evento.

## Consequencias

- o app passa a ajudar tambem na coordenacao do dia de jogo;
- o backend precisa controlar a disponibilidade do codigo;
- o frontend deve oferecer copia simples e clara do codigo;
- o horario exato de liberacao ainda precisa ser fechado.
