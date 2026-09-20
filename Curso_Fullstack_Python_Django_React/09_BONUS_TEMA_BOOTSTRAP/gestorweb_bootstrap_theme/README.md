# GestorWeb Aurora — tema Bootstrap

Tema visual didático para o curso Django. Usa Bootstrap 5.3 por CDN e uma folha CSS própria.

## Instalação rápida

1. Copia `templates/base.html` para a pasta `templates/` do projeto.
2. Copia `templates/components/` para a mesma pasta.
3. Copia `static/css/gestorweb-theme.css` para `static/css/`.
4. Em `settings.py`, confirma `STATIC_URL` e `STATICFILES_DIRS`.
5. Usa `{% extends "base.html" %}` nos templates das apps.
6. Executa o servidor e abre a página do catálogo.

## Paleta

- Navy: `#0F172A`
- Azul: `#2563EB`
- Ciano: `#0891B2`
- Verde: `#16A34A`
- Vermelho: `#DC2626`
- Fundo: `#F8FAFC`

O pacote não contém credenciais, dados privados nem dependências além do Bootstrap carregado por CDN.

---

**Elaborado por Osvaldo Queta — Engenheiro Informático desde 2015 — Programador Sénior com mais de 8 anos de experiência**
