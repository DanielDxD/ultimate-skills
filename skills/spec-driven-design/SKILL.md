---
name: spec-driven-design
description: >-
  Spec-driven design: escreve especificação antes de codar, pede aprovação e
  implementa só o que está na spec. Use sempre que o usuário pedir feature nova,
  spec, SDD, especificação, “antes de implementar”, ou mudanças de produto com
  escopo ambíguo — mesmo sem pedir “spec” explicitamente.
---

# Spec-Driven Design

Nenhuma feature nova sem spec aprovada. Código segue a spec; a spec não segue o código.

## Workflow

1. **Esclarecer** — pergunte o que estiver em dúvida (objetivo, usuários, restrições, fora de escopo).
2. **Escrever a spec** em markdown (arquivo no repo ou bloco claro no chat):
   - Objetivo
   - Escopo / não-escopo
   - Usuários e fluxos principais
   - UI / estados relevantes (se houver interface)
   - Critérios de aceite testáveis
   - Riscos e dependências
3. **Aguardar ok explícito** do usuário. Não implementar antes.
4. **Implementar** apenas o que a spec cobre. Desvios → atualizar a spec e reconfirmar.
5. **Verificar** critérios de aceite ao final.

## Regras

- Nunca pular a spec em features novas.
- Spec curta e verificável > documento longo e vago.
- Se o pedido for trivial (typo, rename local), diga que a spec formal não se aplica e execute direto.
- Em dúvida de escopo: pergunte — não assuma.

## Template mínimo

```markdown
# Spec: <título>

## Objetivo
## Escopo
## Não-escopo
## Fluxos
## UI / estados
## Critérios de aceite
- [ ]
## Dependências / riscos
```
