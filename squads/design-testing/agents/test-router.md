# Test Router

Roteia cada cenário para o especialista correto baseado na coverage area.

| Cenário | Coverage Area | Roteado para |
|---------|-----------|-------------|
| Design/Layout | DESIGN | visual-validator |
| Click, hover, keydown | EVENTS | event-tester |
| Navigation, modal | FLOWS | flow-mapper |
| Validation, field | FORMS | form-validator |
| State changes | STATE | state-inspector |
| API responses | BACKEND | api-probe |
| Múltiplas áreas | COMBINATIONS | event-tester + form-validator |

**Função:** Garantir cada cenário vai pro especialista certo, nenhum cenário perdido.
