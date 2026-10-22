---
name: motion-animation
description: >-
  Motion e animações web com Lenis, GSAP e ScrollTrigger: scroll suave, reveals,
  parallax e microinterações. Use sempre que o usuário pedir animação, motion,
  scroll reveal, pin, stagger, parallax, microinteração ou experiência com
  movimento na página.
---

# Motion & Animation

Stack fixa: **Lenis** (smooth scroll) + **GSAP** + **ScrollTrigger**. Um motor de movimento — não misture Framer Motion, libs de reveal ou smooth scroll em CSS como motor principal.

## Regras

- Entradas/saídas importantes: duração mínima `0.6s` (prefira `0.8–1.4s`).
- Eases: família `power3` ou `expo`. Padrão de entrada: `power3.out`.
- Sequências editoriais: `stagger: 0.2`.
- Anime prioritariamente `transform`, `opacity`, `clip-path`.
- Respeite `prefers-reduced-motion` (desligar ou simplificar motion).
- Preserve a stack do projeto; instale só o que faltar.
- Cleanup de timelines, triggers e Lenis no unmount / ciclo de vida correto.

## Setup mental

1. Lenis controla sensação de scroll.
2. GSAP controla timelines e propriedades.
3. ScrollTrigger liga timelines ao scroll (`pin`, `scrub` quando necessário).
4. Sincronize Lenis com o ticker do GSAP e chame `ScrollTrigger.update`.

## Workflow

1. Definir o papel do motion (atenção, revelação, atmosfera) — não animar por animar.
2. Escolher beats: entrada, sustentação, saída.
3. Implementar com Lenis + GSAP + ScrollTrigger.
4. Testar reduced motion e mobile (reduzir deslocamentos / pin se necessário).

## Checklist

- [ ] Só Lenis + GSAP + ScrollTrigger como motores
- [ ] Durações e eases dentro do padrão
- [ ] `prefers-reduced-motion` tratado
- [ ] Cleanup feito
