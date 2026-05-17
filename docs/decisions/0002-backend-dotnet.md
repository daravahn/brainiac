# ADR 0002: ASP.NET Core no backend

## Status

Proposta aceita para o primeiro corte

## Contexto

O dominio pede:

- regras claras de autorizacao;
- modelagem relacional;
- API consistente para web e mobile;
- espaco para evoluir ranking, validacao e fluxos administrativos.

## Decisao

Usar ASP.NET Core com C# para o backend inicial.

## Consequencias

- autenticacao externa com Google pode seguir os mecanismos oficiais do ecossistema;
- o dominio pode ser organizado em camadas sem abandonar produtividade;
- a API atende Flutter web e mobile pela mesma superficie;
- a escolha do banco continua aberta entre motores relacionais compativeis com o deploy escolhido.
