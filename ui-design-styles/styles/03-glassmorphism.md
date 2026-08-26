# 03 — Glassmorphism

Vidro fosco. Transparência + `backdrop-blur` + borda sutil + camadas.

## Usar quando
Dashboards, SaaS, fundo com foto/gradiente, dark mode premium.

## Cuidado
Legibilidade em tela densa. Blur é caro em device fraco.

## Tailwind
```html
<div class="rounded-3xl border border-white/20 bg-white/10 p-8 backdrop-blur-xl shadow-2xl">
  <h3 class="text-2xl font-semibold text-white">Título</h3>
</div>
```

## Prompt
Crie a interface com vidro fosco forte, hierarquia em camadas, tipografia limpa e contraste AA. HTML + Tailwind.
