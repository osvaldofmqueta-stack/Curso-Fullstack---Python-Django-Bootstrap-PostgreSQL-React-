# Bónus — integrar o tema GestorWeb Aurora

## Objetivo

Aplicar uma identidade visual consistente ao catálogo Django sem reescrever as views ou os models.

## O que está no ZIP

```text
gestorweb_bootstrap_theme/
├── README.md
├── templates/
│   ├── base.html
│   └── components/
├── static/
│   ├── css/gestorweb-theme.css
│   └── js/gestorweb-theme.js
├── preview/tema-preview.svg
└── LICENSE.txt
```

## Passo a passo

1. Descarrega ou extrai `gestorweb_bootstrap_theme.zip`.
2. Copia `templates/base.html` para a pasta `templates/` do projeto.
3. Copia `templates/components/` para dentro de `templates/`.
4. Copia `static/css/gestorweb-theme.css` para `static/css/`.
5. Confirma em `settings.py` que `BASE_DIR / "templates"` e `BASE_DIR / "static"` estão configurados.
6. Em cada página, usa `{% extends "base.html" %}`.
7. Mantém o `{% block content %}` para o conteúdo da página.
8. Executa `python manage.py check` e abre a aplicação.

## Exemplo de página

```html
{% extends "base.html" %}

{% block title %}Produtos | GestorWeb{% endblock %}

{% block content %}
<h1 class="mb-4">Produtos</h1>
<div class="card gw-card p-4">
  O conteúdo específico desta página fica aqui.
</div>
{% endblock %}
```

## Verificação visual

- Navbar navy aparece.
- Fundo da aplicação é claro.
- Botões principais são azuis.
- Produtos disponíveis usam verde.
- Erros e stock esgotado usam vermelho.
- A página continua utilizável no telemóvel.

O preview é um wireframe ilustrativo. A aparência final depende dos dados e templates do teu projeto.

---

**Elaborado por Osvaldo Queta — Engenheiro Informático desde 2015 — Programador Sénior com mais de 8 anos de experiência**
