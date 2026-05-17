# ADR 0001: Flutter multiplataforma no frontend

## Status

Aceita

## Contexto

O produto precisa atender dois grupos desde cedo:

- jogadores, que terao valor no celular para inscricao, consulta de mesa, ranking e copia do codigo da Wizard;
- organizador e conselho, que precisam de uma experiencia administrativa forte no navegador.

## Decisao

Usar Flutter como frontend unico para web, Android e iOS desde o inicio.

## Consequencias

- teremos uma base de codigo compartilhada entre plataformas;
- a experiencia web precisara ser tratada com cuidado proprio, especialmente para telas administrativas;
- a experiencia do jogador pode nascer mobile-first sem adiar a chegada em iOS e Android;
- componentes e navegacao devem ser desenhados de forma adaptativa, nao apenas responsiva.
