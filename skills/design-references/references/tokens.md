# Tokens de design

Base `4`. Spacing, sizing e radius só em múltiplos de 4 (única exceção: `radius-full`).

## Escala permitida

`4, 8, 12, 16, 20, 24, 32, 40, 48, 64, 80, 96, 128…`

## Space

| Token | Valor |
|-------|-------|
| `--space-1` | `4px` |
| `--space-2` | `8px` |
| `--space-3` | `12px` |
| `--space-4` | `16px` |
| `--space-5` | `20px` |
| `--space-6` | `24px` |
| `--space-7` | `32px` |
| `--space-8` | `40px` |
| `--space-9` | `48px` |
| `--space-10` | `64px` |
| `--space-11` | `80px` |
| `--space-12` | `96px` |

Gaps de seção e padding de layout usam esta escala.

## Radius

| Token | Valor |
|-------|-------|
| `--radius-none` | `0` |
| `--radius-sm` | `4px` |
| `--radius-md` | `8px` |
| `--radius-lg` | `12px` |
| `--radius-xl` | `16px` |
| `--radius-2xl` | `24px` |
| `--radius-full` | `9999px` |

## Size

Alturas de controle, ícones e alvos de toque — mesma escala:

| Token | Valor | Uso típico |
|-------|-------|------------|
| `--size-icon-sm` | `16px` | ícone compacto |
| `--size-icon` | `20px` | ícone padrão |
| `--size-icon-lg` | `24px` | ícone destaque |
| `--size-control-sm` | `32px` | control compacto |
| `--size-control` | `40px` | botão / input |
| `--size-control-lg` | `48px` | control largo |

Tipografia em `px`/`rem` também ancora em múltiplos de 4 (ex.: 12 / 16 / 20 / 24 / 32 / 40 / 48 / 64).

## Camadas

```css
:root {
  /* Primitive */
  --color-neutral-0: #ffffff;
  --color-neutral-50: #f7f7f5;
  --color-neutral-100: #ecece8;
  --color-neutral-400: #8a8a84;
  --color-neutral-800: #1c1c1a;
  --color-neutral-900: #111110;
  --color-accent-raw: #2f6f5e; /* do brief / referências */

  /* Semantic */
  --color-bg: var(--color-neutral-50);
  --color-surface: var(--color-neutral-0);
  --color-fg: var(--color-neutral-900);
  --color-muted: var(--color-neutral-400);
  --color-border: var(--color-neutral-100);
  --color-accent: var(--color-accent-raw);
  --color-accent-fg: #ffffff;
  --color-danger: #b42318;
  --color-success: #1f7a4c;

  /* Component (só se necessário) */
  --button-bg: var(--color-accent);
  --button-fg: var(--color-accent-fg);
  --button-radius: var(--radius-md);
}
```

## Paleta

Papéis semânticos obrigatórios: `bg`, `surface` (opcional elevated), `fg`, `muted`, `border`, `accent`, `accent-fg`, `danger`, `success`.

1. Partir dos neutros acima (ou adaptar light/dark do brief).
2. Definir `accent` a partir do brief e das referências — documentar **4–6 cores nomeadas** (hex nos primitives) antes do código.
3. Na UI, usar só tokens semânticos/component — nunca hex soltos.

## Checklist antes do código

- [ ] Nenhum spacing/sizing fora da escala de múltiplos de 4
- [ ] Radius só via `--radius-*`
- [ ] Cores só via semantic/component
- [ ] Accent documentado e ligado a `--color-accent`
