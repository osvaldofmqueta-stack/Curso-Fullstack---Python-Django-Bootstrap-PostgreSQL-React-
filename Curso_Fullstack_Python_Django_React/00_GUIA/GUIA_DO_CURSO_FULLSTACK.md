# Curso Fullstack — Python, Django, APIs e React

## Objetivo do curso

Construir uma aplicação real de gestão de catálogo e evoluí-la até uma aplicação full-stack:

```text
Python
  ↓
Django Templates + Bootstrap
  ↓
PostgreSQL
  ↓
Django REST Framework
  ↓
React
  ↓
Testes, segurança e publicação
```

O projeto-guia é um **Catálogo Web**. Ele começa com produtos e categorias e pode evoluir para clientes, vendas, relatórios e gestão para pequenos negócios.

---

## Como estão organizadas as pastas

```text
Curso_Fullstack_Python_Django_React/
├── 00_GUIA/
│   └── GUIA_DO_CURSO_FULLSTACK.md
├── 01_FUNDAMENTOS_DJANGO/
│   ├── Aula_1 — Primeiro projeto
│   └── Aula_2 — Models, migrations e Admin
├── 02_WEB_COM_DJANGO/
│   ├── Aula_3 — URLs, Views e Templates
│   ├── Aula_4 — Django ORM
│   └── Aula_5 — HTML, CSS e Bootstrap
├── 03_APLICACAO_E_QUALIDADE/
│   ├── Aula_6 — Formulários e CRUD
│   ├── Aula_7 — Autenticação e permissões
│   └── Aula_8 — Testes automatizados
├── 04_RELATORIOS_E_EXPORTACAO/
│   ├── Aula_9 — Relatórios e dashboard
│   ├── Aula_10 — Exportação Excel
│   └── Aula_11 — Geração de PDF
├── 05_DADOS_E_APIS/
│   └── Aula_12 — PostgreSQL e configuração
├── 06_FRONTEND_REACT/
└── 07_PROJETO_FINAL_E_DEPLOY/
```

As pastas 06 e 07 ficam reservadas para as próximas etapas do curso.

---

## Método de estudo

Cada aula deve durar aproximadamente duas horas:

| Parte | Tempo | Como trabalhar |
|---|---:|---|
| Compreender | 20 min | Ler o conceito e explicar o fluxo. |
| Construir | 50 min | Escrever os ficheiros e executar os comandos. |
| Exercitar | 35 min | Resolver sem copiar a solução. |
| Rever | 15 min | Corrigir, testar e registar o que aprendeste. |

Não avances apenas porque terminaste a leitura. Avança quando conseguires:

1. Explicar o conceito com as tuas palavras.
2. Alterar o exemplo sem copiar tudo.
3. Corrigir pelo menos um erro.
4. Resolver o exercício principal.
5. Fazer um pequeno commit no Git.

---

## Bibliotecas: o que usar e quando

| Necessidade | Biblioteca escolhida | Quando usar | Por que esta escolha |
|---|---|---|---|
| Backend web | Django | Desde a Aula 1 | Framework completo e adequado para aprender Python web. |
| Interface inicial | Bootstrap 5 | A partir da Aula 5 | Responsivo, documentado e simples para começar. |
| Testes | Django TestCase | Aula 8 | Já vem com Django e ensina os fundamentos. |
| Testes maiores | pytest + pytest-django | Depois da Aula 8 | Sintaxe agradável e boa organização. |
| Excel | openpyxl | Aula 10 | Direto para criar e formatar `.xlsx`. |
| PDF | WeasyPrint | Aula 11 | Reutiliza HTML e CSS dos templates. |
| Base de dados | PostgreSQL | Aula 12 | Mais adequado para produção e dados relacionais. |
| Driver PostgreSQL | psycopg | Aula 12 | Liga Python ao PostgreSQL. |
| Configuração | variáveis de ambiente | Aula 12 | Mantém segredos fora do código. |
| API | Django REST Framework | Aula 15 | Integração madura com Django. |
| Frontend | React + Vite | Aula 18 | Componentes e desenvolvimento moderno. |
| HTTP no frontend | `fetch` primeiro | Aula 19 | Aprende o fundamento antes de adicionar outra biblioteca. |
| Interações simples | HTMX, mais tarde | Depois do Django sólido | Adiciona dinamismo sem saltar logo para React. |

### Decisões simples para não te dispersares

- Não trocar Bootstrap por Tailwind no início. Tailwind é poderoso, mas não é mais simples para quem está a aprender.
- Não usar React antes de compreender Templates Django, HTML e formulários.
- Não usar Pandas para um Excel simples. Primeiro aprende `openpyxl`.
- Não começar por PDF. Primeiro cria o relatório no navegador; depois exporta para Excel e PDF.
- Não usar PostgreSQL antes de compreender models, migrations e ORM com SQLite.
- Não adicionar muitas bibliotecas para resolver problemas que o Django já resolve.

---

## Roadmap completo das próximas aulas

### Fase 1 — Django básico

#### Aulas 1–2

- Criar ambiente virtual e projeto.
- Entender `manage.py`.
- Criar apps.
- Criar models.
- Aplicar migrations.
- Usar SQLite.
- Registar models no Admin.

**Resultado:** um backend de catálogo com categorias e produtos.

### Fase 2 — Web com Django

#### Aulas 3–5

- URLs, views e templates.
- Ciclo request → view → ORM → template.
- HTML básico dentro dos templates.
- CSS fundamental.
- Bootstrap.
- Layout responsivo.

**Resultado:** uma página pública do catálogo com identidade visual.

### Fase 3 — Aplicação funcional e qualidade

#### Aulas 6–8

- Formulários e `ModelForm`.
- Criar, editar e apagar produtos.
- CSRF e mensagens.
- Registo, login e logout.
- Staff e permissões.
- Testes de models, views e formulários.

**Resultado:** uma aplicação funcional, protegida e testada.

### Fase 4 — Relatórios e exportação

#### Aulas 9–11

- Dashboard.
- `Count`, `Sum`, `Avg`, `Min`, `Max`.
- Relatórios de stock e preços.
- Excel com `openpyxl`.
- PDF com WeasyPrint.

**Resultado:** informação útil para decisão e ficheiros descarregáveis.

### Fase 5 — Base de dados e APIs

#### Aulas 12–15

#### Aula 12 — PostgreSQL e configuração

- PostgreSQL.
- `psycopg`.
- Variáveis de ambiente.
- Backups.
- Migrations em ambientes diferentes.

#### Aula 13 — Segurança Django

- `DEBUG`.
- `ALLOWED_HOSTS`.
- CSRF.
- Passwords.
- Ficheiros estáticos.
- Ficheiros de media.
- Configuração de produção.

#### Aula 14 — Django REST Framework

- Serializers.
- APIViews.
- ViewSets.
- Routers.
- JSON.
- Métodos GET, POST, PUT e DELETE.

#### Aula 15 — API profissional

- Paginação.
- Filtros.
- Pesquisa.
- Permissões.
- Autenticação de API.
- Documentação dos endpoints.

**Resultado:** uma API Django pronta para ser consumida por outro frontend.

### Fase 6 — Frontend moderno

#### Aulas 16–20

#### Aula 16 — JavaScript essencial

- Variáveis.
- Funções.
- Arrays.
- Objetos.
- Eventos.
- `fetch`.
- JSON.

#### Aula 17 — React básico

- Projeto com Vite.
- Componentes.
- JSX.
- Props.
- Estado.
- Eventos.

#### Aula 18 — React aplicado

- Listas.
- Formulários.
- React Router.
- Loading.
- Mensagens de erro.
- Bootstrap no React.

#### Aula 19 — React ligado ao Django

- Consumir a API.
- Listar produtos.
- Criar produtos.
- Editar produtos.
- Apagar produtos.
- Enviar tokens ou sessão com segurança.

#### Aula 20 — Dashboard React

- Layout da aplicação.
- Navbar.
- Tabelas.
- Filtros.
- Gráficos.
- Estados vazios.
- Estados de carregamento.

**Resultado:** frontend React ligado à API Django.

### Fase 7 — Projeto final e publicação

#### Aulas 21–28

#### Aula 21 — Planeamento

- Escolher o problema.
- Definir utilizadores.
- Listar funcionalidades.
- Desenhar as páginas.
- Definir models e relações.

#### Aula 22 — Backend do projeto

- Models.
- Migrations.
- Admin.
- Serviços.
- Validação.

#### Aula 23 — Autenticação e permissões

- Perfis de utilizador.
- Grupos.
- Permissões.
- Áreas privadas.

#### Aula 24 — API do projeto

- Endpoints.
- Serializers.
- Filtros.
- Paginação.
- Documentação.

#### Aula 25 — Frontend do projeto

- Componentes.
- Rotas.
- Formulários.
- Integração com API.

#### Aula 26 — Relatórios e dashboard

- Indicadores.
- Exportação.
- Gráficos.
- Filtros por datas.

#### Aula 27 — Testes e segurança

- Testes backend.
- Testes frontend.
- Validação.
- Segredos.
- CORS.
- Erros.

#### Aula 28 — Deploy e portfólio

- Preparar produção.
- Configurar base de dados.
- Recolher ficheiros estáticos.
- Publicar.
- Ler logs.
- Criar README.
- Apresentar o projeto no GitHub.

**Resultado final:** uma aplicação full-stack publicada e apresentável no portfólio.

---

## Quando podes considerar que mudaste de nível?

### Django básico

Depois da Aula 8, se conseguires construir e testar uma aplicação simples sem copiar todos os passos.

### Django intermédio

Depois das Aulas 12–15, quando conseguires trabalhar com PostgreSQL, APIs, permissões, relatórios e configuração de produção.

### Full-stack intermédio

Depois da Aula 20, quando conseguires ligar um frontend React a uma API Django.

### Programador full-stack avançado

Depois de terminares um projeto real, o publicares, o protegeres, escreveres testes e conseguires diagnosticar problemas de produção.

O número da aula é apenas um guia. A competência é medida pelo que consegues construir e explicar.

---

## Regra de progressão

Não aprender tudo ao mesmo tempo. A ordem recomendada é:

```text
Python
→ HTML e CSS
→ Django Templates
→ Bootstrap
→ Models e ORM
→ CRUD
→ Login e permissões
→ Testes
→ Relatórios
→ PostgreSQL
→ APIs
→ JavaScript
→ React
→ Deploy
```

Esta ordem reduz a complexidade e permite que cada tecnologia resolva um problema que já compreendes.

---

## Projeto ZIP de cada aula

Cada aula tem um pacote de prática em:

```text
10_PROJETOS_ZIPADOS_POR_AULA/
```

Dentro de cada ZIP existem:

```text
STARTER/
EXPECTED/
ESTADO_ESPERADO.md
CHECKLIST.md
```

Usa `STARTER` para começar a construir. Abre `EXPECTED` apenas depois da tua tentativa, para comparar a estrutura e corrigir o que falta. Os ZIPs são referências didáticas progressivas; a implementação final deve ser executada e validada por ti no teu projeto.

## Material extra

- `00_GUIA/GUIA_VISUAL_APLICACAO.md` — wireframes da evolução do GestorWeb.
- `00_GUIA/PROJETO_EM_CONSTRUCAO.md` — motivação e marcos visuais do projeto.
- `08_APLICACOES_COMPLETAS/` — TaskFlow, ContactFlow CRM e ReservaFácil.
- `09_BONUS_TEMA_BOOTSTRAP/` — tema Bootstrap e pacote ZIP reutilizável.

---

**Elaborado por Osvaldo Queta — Engenheiro Informático desde 2015 — Programador Sénior com mais de 8 anos de experiência**
