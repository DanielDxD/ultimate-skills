---
name: design-consistency
description: >-
  Garante design e consistência visual: tokens, ritmo de espaçamento, componentes
  reutilizados e UI uniforme. Use sempre que o usuário pedir design system,
  consistência visual, padronizar UI, tokens, tipografia/cor alinhadas, ou ao
  criar várias telas/seções que precisam parecer do mesmo produto.
---

# Design Consistency

Visual e interação devem parecer um sistema, não páginas soltas. Complementa `design-references` (galerias + tokens base); não substitui a pesquisa de referências.

## Regras

- Espaçamento, sizing e radius só em **múltiplos de 4** — seguir [`../design-references/references/tokens.md`](../design-references/references/tokens.md).
- Cores e tipografia só via tokens (primitive → semantic → component); sem hex soltos em componentes.
- Preferir componentes existentes a one-offs; se criar um novo, reutilize-o na próxima ocorrência.
- Mesmos padrões de hierarquia tipográfica, botões, cards e estados (hover/focus/disabled) em todo o produto.
- Em site/landing: antes de inventar visual, aplique o ritual de `design-references`.

## Workflow

1. Inventariar tokens e componentes já no projeto.
2. Se for página/marketing: buscar referências (`design-references`).
3. Declarar ou estender tokens (space, radius, size, cor) antes do CSS ad-hoc.
4. Implementar reutilizando o sistema; extrair componente se o padrão se repetir.
5. Revisar consistência: gaps, radii, pesos tipográficos e estados.

## Checklist

- [ ] Nada fora da escala de 4px
- [ ] Cores só por token semântico
- [ ] Componentes repetidos, não clones com CSS diferente
- [ ] Referências consultadas quando aplicável
