---
name: roadmap
description: >-
  Monta roadmaps checkáveis em fases para o projeto completo (não só MVP) em
  implementações grandes. Use sempre que o usuário pedir roadmap, plano de
  fases, implementação grande, projeto do zero, “como vamos construir”,
  epic, milestone, ou antes de começar um trabalho amplo — mesmo sem pedir
  “roadmap” explicitamente.
---

# Roadmap

Em implementações grandes, **sempre** entregue um roadmap checkável antes (ou no início) da execução. O roadmap cobre o **projeto inteiro em fases** — não pare no MVP.

Complementa `spec-driven-design`: a spec detalha o que construir; o roadmap ordena **quando** e em qual fase. Em dúvida, pergunte.

## Quando aplicar

- Projeto novo, redesign amplo, migração, plataforma multi-módulo
- Feature grande que toca várias camadas ou times
- Pedidos do tipo “vamos construir X” sem ordem clara

**Não** use roadmap formal para typos, bugs pontuais ou mudanças locais triviais — diga que não se aplica e execute.

## Regras

- Fases do **produto completo**, não só “MVP e depois a gente vê”.
- Cada item é um checkbox `- [ ]` verificável (feito / não feito).
- Cada fase tem: objetivo, entregáveis checkáveis, dependências, critério de “fase pronta”.
- Ordem por valor e dependência técnica — não por tamanho de arquivo.
- MVP pode ser a **Fase 1**, mas as fases seguintes (hardening, escala, polish, ops) entram no mesmo documento desde o início.
- Atualize checkboxes conforme o progresso; não abandone o roadmap no meio.
- Em dúvida de escopo ou prioridade: **pergunte** antes de inventar.

## Workflow

1. **Mapear o destino** — visão do produto completo (não só o primeiro release).
2. **Dividir em fases** — tipicamente 4–7 (ex.: fundação → core → expansão → qualidade → escala → polish). Ajuste ao brief.
3. **Escrever o roadmap** (arquivo preferencial: `docs/roadmap.md`, ou caminho que o usuário pedir) com o template abaixo.
4. **Confirmar** com o usuário a ordem e o que entra em cada fase.
5. **Executar** fase a fase; marcar `- [x]` ao concluir itens; só avance de fase quando o critério de saída for atendido (ou o usuário autorizar).

## Template

```markdown
# Roadmap: <projeto>

## Visão
<1–3 frases do produto completo>

## Fase 0 — Descoberta / alinhamento
**Objetivo:** …
**Critério de saída:** …
- [ ] …
- [ ] …

## Fase 1 — Fundação
**Objetivo:** …
**Dependências:** …
**Critério de saída:** …
- [ ] …
- [ ] …

## Fase 2 — Core do produto
**Objetivo:** …
**Dependências:** Fase 1
**Critério de saída:** …
- [ ] …
- [ ] …

## Fase 3 — Expansão
**Objetivo:** …
**Dependências:** Fase 2
**Critério de saída:** …
- [ ] …
- [ ] …

## Fase 4 — Qualidade e hardening
**Objetivo:** testes, acessibilidade, performance, segurança básica
**Critério de saída:** …
- [ ] …
- [ ] …

## Fase 5 — Escala e operação
**Objetivo:** observabilidade, deploys, docs, handoff
**Critério de saída:** …
- [ ] …
- [ ] …

## Fase 6 — Polish / diferenciação
**Objetivo:** motion, 3D, brand extras, delighters — se no escopo do produto
**Critério de saída:** …
- [ ] …

## Fora deste roadmap (backlog explícito)
- [ ] … (itens conscientes de “depois”, não esquecidos)
```

Adapte nomes e quantidade de fases ao projeto; mantenha checkboxes e critérios de saída.

## Checklist do agente

- [ ] Roadmap cobre além do MVP
- [ ] Itens checkáveis e critérios de saída por fase
- [ ] Usuário confirmou (ou ajustou) antes de executar em massa
- [ ] Progresso refletido nos checkboxes
