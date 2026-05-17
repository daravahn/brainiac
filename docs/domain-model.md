# Modelo de dominio

## Entidades principais

### Player

- id
- nome
- email
- ativo
- role

### Season

- id
- nome
- data_inicio
- data_fim
- status

### Event

- id
- season_id
- data
- tema
- is_deck_swap_day
- wizard_event_code
- wizard_event_code_available_at
- status

### EventRegistration

- id
- event_id
- player_id
- confirmou_presenca
- pedido_vault
- pagamento_confirmado
- deck_id
- deck_status
- submitted_at

### Deck

- id
- owner_player_id
- nome
- commander
- url
- status_validacao

### Round

- id
- event_id
- numero
- status

### Pod

- id
- round_id
- numero_mesa

### PodPlayer

- id
- pod_id
- player_id
- deck_id

### PodResult

- id
- pod_id
- player_id
- colocacao
- eliminado_antes_do_empate
- pontos_base
- pontos_bonus

### ResultValidation

- id
- pod_id
- submitted_by
- validated_by
- status
- validated_at

## Projecoes derivadas

### EventStanding

Calculado a partir de resultados validados dentro de um evento.

### SeasonStanding

Calculado a partir de resultados validados em todos os eventos da season.

## Observacoes de modelagem

- Rankings devem ser derivados de resultados validados, evitando dupla fonte de verdade.
- `Deck` separado de `EventRegistration` permite reutilizar o mesmo deck em varios eventos.
- `PodPlayer` precisa registrar qual deck foi usado naquela mesa para suportar futuras regras de troca de decks.
- `Player.role` deve cobrir pelo menos jogador, admin_conselho e admin_geral no primeiro backend.
- O codigo da Wizard pertence ao `Event` e deve ter uma janela de disponibilidade controlada pelo backend.
