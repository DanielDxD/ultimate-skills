---
name: design-references
description: >-
  Obriga pesquisa de referências em Minimal Gallery, CollectUI, BentoGrids e
  Footer Design, e aplicação de tokens de design (espaçamento/radius em múltiplos
  de 4, tamanhos e paleta semântica) antes de projetar ou redesenhar websites e
  seções. Use sempre que o usuário pedir site, landing page, portfólio,
  e-commerce, hero, footer, bento, grid de features, UI, animação, redesign,
  inspiração visual, direção de arte ou sistema de tokens — mesmo sem pedir
  “referências” explicitamente.
---

# Design References

Antes de definir direção visual ou escrever UI, consulte as galerias, escolha a melhor fonte por seção e declare tokens. Preserve a stack e as skills de implementação existentes; esta skill fixa referências + tokens, não o framework.

## Escolher a melhor fonte

| Precisa de… | Fonte | URL |
|-------------|-------|-----|
| Direção de site / landing / portfólio (página inteira) | Minimal Gallery — **obrigatória** | https://minimal.gallery |
| UI de produto, componentes, microinterações, motion | CollectUI (+ Minimal se for página) | https://collectui.com |
| Bento / feature grid / cards densos | BentoGrids | https://bentogrids.com |
| Footer | Footer Design (preferir Editor's Choice) | https://footer.design |

Combinação de seções → Minimal Gallery + fontes das seções envolvidas. Ainda assim, **2–4 referências no total**.

Detalhes de tags, filtros e critérios: [references/sources.md](references/sources.md).

## Workflow

1. **Mapear o brief** — tipo de página e seções (hero, features/bento, UI, footer, etc.).
2. **Escolher fontes** — use a árvore acima. Em site/landing, Minimal Gallery é obrigatória.
3. **Buscar de verdade** — WebFetch ou browser nas URLs reais. Leia [references/sources.md](references/sources.md). Não invente entradas.
4. **Selecionar 2–4 referências** alinhadas ao brief. Em Minimal Gallery, abra pelo menos uma `/site/<slug>/` quando útil.
5. **Extrair notas concretas** — layout, tipografia, cor, densidade, motion, hierarquia. Não copiar marca, copy nem assets.
6. **Tokenizar** — leia [references/tokens.md](references/tokens.md). Declare CSS variables (primitive → semantic → component): space, radius, size e cores. Só múltiplos de 4 (exceto `radius-full`). Hex apenas nos primitives; UI usa só tokens semânticos/component.
7. **Implementar** — cite as URLs das referências e use só a escala tokenizada.
8. **Fallback** — se uma galeria falhar, tente outra da lista e/ou a homepage; registre o bloqueio. Nunca fabrique referências falsas.

## Regras

- Não pule a pesquisa porque “já conhece o estilo”.
- Não use `px` de spacing/sizing/radius fora da escala de múltiplos de 4.
- Não use hex soltos em componentes — só via tokens.
- Não embuta screenshots ou assets copiados das galerias.
