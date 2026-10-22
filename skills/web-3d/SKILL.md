---
name: web-3d
description: >-
  Cenas 3D na web com Three.js e React Three Fiber (R3F): performance,
  fallbacks e acessibilidade. Use sempre que o usuário pedir 3D, WebGL,
  Three.js, R3F, cena 3D, modelo interativo ou hero tridimensional.
---

# Web 3D

Stack: **Three.js**. Em React: **@react-three/fiber** + **@react-three/drei**.

## Regras

- Lazy-load da cena 3D; não bloquear LCP com o bundle WebGL.
- Limitar lights, materiais caros e polígonos; preferir instancing quando houver muitos objetos iguais.
- Pause / dispose fora do viewport (IntersectionObserver ou equivalente).
- Fallback 2D (imagem/vídeo estático) se WebGL falhar ou `prefers-reduced-motion`.
- Controles acessíveis: não dependa só de drag 3D para informação crítica.
- Preserve a arquitetura do app; isole a cena em um boundary de cliente (SSR).

## Workflow

1. Definir o job da cena (hero atmosférico, produto, exploração) e o fallback 2D.
2. Escolher vanilla Three.js ou R3F conforme a stack do repo.
3. Implementar cena mínima → medir → só então adicionar efeitos.
4. Garantir dispose de geometrias, materiais e renderer no unmount.
5. Validar mobile, reduced motion e LCP.

## Checklist

- [ ] Lazy-load + sem bloquear LCP
- [ ] Fallback 2D / reduced motion
- [ ] Pause fora do viewport + dispose
- [ ] Cena isolada do resto do app
