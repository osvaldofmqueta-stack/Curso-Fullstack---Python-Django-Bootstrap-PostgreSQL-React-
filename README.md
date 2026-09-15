# Curso Fullstack — Python, Django, Bootstrap, PostgreSQL e React

Roteiro completo para aprender desenvolvimento web full-stack através de uma stack prática:

```text
Python + Django + Bootstrap + PostgreSQL + Django REST Framework + React
```

O curso foi pensado para estudar 5 dias por semana, 2 horas por dia, durante 24 semanas. O objetivo é terminar com capacidade para criar, testar, publicar e explicar aplicações web completas.

## Stack do curso

- **Python** — lógica e programação
- **HTML** — estrutura das páginas
- **CSS** — fundamentos visuais
- **Bootstrap** — framework de estilização fácil para começar
- **JavaScript** — interatividade no navegador
- **Django** — backend e aplicações web
- **SQLite** — primeira base de dados
- **PostgreSQL** — base de dados para produção
- **Django REST Framework** — criação de APIs
- **React** — frontend moderno
- **Git e GitHub** — controlo de versões e portfólio
- **pytest e testes Django** — qualidade do código

## Ritmo de estudo

- 5 dias por semana
- 2 horas por dia
- 10 horas por semana
- 24 semanas
- Aproximadamente 240 horas

### Estrutura de cada aula — 120 minutos

| Atividade | Tempo |
|---|---:|
| Revisão da aula anterior | 10 min |
| Explicação do novo conteúdo | 20 min |
| Exemplo acompanhado | 35 min |
| Exercício individual | 40 min |
| Corrigir erros e fazer commit | 15 min |
| **Total** | **120 min** |

À sexta-feira, o estudo é dedicado à revisão, ao projeto da semana, aos testes, à correção de erros e ao GitHub.

## Instalações por etapa

Não é necessário instalar tudo no primeiro dia.

### Antes da primeira aula

Instalar:

1. Google Chrome
2. Visual Studio Code
3. Python
4. Git
5. Criar uma conta no GitHub

Confirmar no terminal:

```bash
python --version
git --version
```

Em alguns computadores, o comando do Python é:

```bash
python3 --version
```

### Criar um ambiente virtual Python

Dentro de cada projeto Python:

```bash
python -m venv .venv
```

Windows:

```bash
.venv\Scripts\activate
```

macOS/Linux:

```bash
source .venv/bin/activate
```

Depois:

```bash
python -m pip install --upgrade pip
```

### Quando começar Django

```bash
python -m pip install django
```

### Quando começar PostgreSQL

Instalar:

- PostgreSQL
- pgAdmin

SQLite será utilizado no início porque já vem integrado ao Django.

### Quando começar APIs

```bash
python -m pip install djangorestframework
```

Para testar APIs, utilizar Thunder Client no VS Code ou Postman.

### Quando começar React

Instalar a versão LTS do Node.js e confirmar:

```bash
node --version
npm --version
```

Criar um projeto React:

```bash
npm create vite@latest frontend
cd frontend
npm install
npm run dev
```

# Plano de 24 semanas

## Semanas 1–4 — Python

### Ferramentas

- Python
- VS Code
- Terminal
- Git
- GitHub

### Conteúdos

- Variáveis, strings e números
- Operadores
- Condições
- Ciclos
- Funções
- Listas, dicionários, tuplos e conjuntos
- Ficheiros
- JSON
- Exceções
- Organização de código

### Exercícios

- Calculadora
- Conversor de idade e temperatura
- Tabuada
- Sistema de notas
- Lista de contactos
- Sistema de produtos

### Projeto

**Gestor financeiro no terminal**

- Registar receitas
- Registar despesas
- Calcular saldo
- Listar movimentos
- Guardar dados em JSON

## Semanas 5–8 — HTML, CSS, Bootstrap e JavaScript

### Semana 5 — HTML

Estudar estrutura HTML, títulos, parágrafos, links, imagens, listas, tabelas, formulários e elementos semânticos.

Exercícios:

- Página pessoal
- Formulário de contacto
- Página de hobbies
- Tabela de preços

### Semana 6 — CSS

Estudar cores, fontes, margens, espaçamentos, bordas, Flexbox, Grid e responsividade.

Exercícios:

- Cartão de perfil
- Barra de navegação
- Galeria de imagens
- Página adaptada para telemóvel

### Semana 7 — Bootstrap

Bootstrap será o framework de estilização principal do curso. Primeiro serão estudados os fundamentos de CSS, para que as classes do Bootstrap não sejam utilizadas de forma mecânica.

Adicionar ao HTML:

```html
<link
  href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css"
  rel="stylesheet">
```

Estudar:

- Containers
- Grid
- Botões
- Cards
- Navbar
- Formulários
- Alertas
- Modais
- Tabelas
- Classes responsivas

### Semana 8 — JavaScript no navegador

Estudar variáveis, funções, arrays, objetos, DOM, eventos, validação de formulários e `localStorage`.

Exercícios:

- Contador
- Menu abrir/fechar
- Tema claro/escuro
- Formulário com validação
- Lista de tarefas

### Projeto

**Portfólio pessoal responsivo**

- Página inicial
- Sobre mim
- Competências
- Projetos
- Contacto
- Bootstrap
- Design para computador e telemóvel

Publicar no GitHub.

## Semanas 9–12 — Django fundamental

### Semana 9 — Primeiro projeto Django

Instalar:

```bash
python -m pip install django
```

Criar o projeto:

```bash
django-admin startproject config .
python manage.py startapp core
python manage.py runserver
```

Estudar projetos, aplicações, servidor, URLs, views e templates.

Exercícios:

- Página inicial
- Página “Sobre”
- Página de contacto
- Menu entre páginas

### Semana 10 — Templates e Bootstrap no Django

Estudar:

- Herança de templates
- `base.html`
- Blocos
- Ficheiros estáticos
- CSS no Django
- Bootstrap em templates

Estrutura recomendada:

```text
projeto/
├── config/
├── core/
├── templates/
│   ├── base.html
│   ├── home.html
│   └── contacto.html
├── static/
│   ├── css/
│   └── js/
└── manage.py
```

### Semana 11 — Models e Django Admin

Estudar models, campos, migrations, SQLite, Django Admin e ORM.

Comandos:

```bash
python manage.py makemigrations
python manage.py migrate
python manage.py createsuperuser
python manage.py runserver
```

### Semana 12 — Projeto

**Blog pessoal com Django e Bootstrap**

- Criar artigos pelo admin
- Listar artigos
- Ver artigo completo
- Categorias
- Pesquisa
- Layout responsivo
- Página de contacto

## Semanas 13–15 — Bases de dados e autenticação

### Semana 13 — PostgreSQL

Estudar tabelas, colunas, relações, SQL básico, PostgreSQL com Django e migrations.

Exercícios:

- Tabela de produtos
- Tabela de categorias
- Relação entre produtos e categorias
- Pesquisa e filtros

### Semana 14 — Formulários Django

Estudar Django Forms, ModelForms, validação, mensagens e operações de criar, editar e apagar.

### Semana 15 — Login e permissões

Estudar registo, login, logout, sessões, perfis, permissões e páginas privadas.

### Projeto

**Sistema de gestão de tarefas**

- Criar conta
- Iniciar sessão
- Criar tarefas
- Editar tarefas
- Apagar tarefas
- Marcar como concluídas
- Cada utilizador vê apenas as suas tarefas
- Interface feita com Bootstrap

## Semanas 16–18 — APIs e React

### Semana 16 — Django REST Framework

Instalar:

```bash
python -m pip install djangorestframework
```

Estudar APIs REST, JSON, serializers, views de API, ViewSets, routers e métodos GET, POST, PUT e DELETE.

Exercícios:

- API de produtos
- API de tarefas
- API de utilizadores
- Testar endpoints com Thunder Client

### Semana 17 — React básico

Instalar Node.js LTS e criar o projeto:

```bash
npm create vite@latest frontend
cd frontend
npm install
npm run dev
```

Estudar componentes, JSX, props, estado, eventos, formulários, listas e React Router.

### Semana 18 — React ligado ao Django

Estudar `fetch`, comunicação com a API, criação, edição e eliminação de dados e login no React.

### Projeto

**Dashboard React para a API Django**

- Listar produtos
- Adicionar produtos
- Editar produtos
- Apagar produtos
- Pesquisar
- Filtrar
- Interface com Bootstrap

## Semanas 19–20 — Testes, segurança e publicação

### Semana 19 — Testes

Instalar:

```bash
python -m pip install pytest pytest-django
```

Estudar testes de models, views, APIs, formulários e autenticação.

### Semana 20 — Publicação

Estudar:

- Variáveis de ambiente
- Segurança de passwords
- Ficheiros estáticos
- Ficheiros de media
- Configuração de produção
- GitHub
- Deploy

Publicar:

```text
React → Django REST Framework → PostgreSQL
```

## Semanas 21–24 — Projeto final

### Projeto recomendado

**Sistema de gestão para pequenos negócios**

Tecnologias:

- Python
- Django
- Bootstrap
- PostgreSQL
- Django REST Framework
- React
- GitHub

Funcionalidades:

- Registo e login
- Clientes
- Produtos ou serviços
- Vendas ou reservas
- Dashboard
- Pesquisa
- Filtros
- Relatórios
- Permissões
- API
- Frontend React
- Base de dados PostgreSQL

### Semana 21 — Planeamento

- Definir o problema
- Listar funcionalidades
- Desenhar as páginas
- Criar os modelos da base de dados
- Criar o repositório GitHub

### Semana 22 — Backend

- Criar projeto Django
- Criar models
- Criar migrations
- Criar autenticação
- Criar endpoints da API

### Semana 23 — Frontend

- Criar páginas React
- Adicionar Bootstrap
- Ligar à API
- Criar formulários
- Criar dashboard

### Semana 24 — Finalização

- Testar
- Corrigir erros
- Melhorar o design
- Criar README
- Publicar
- Adicionar o projeto ao portfólio

# Tecnologias a evitar no início

Para manter o foco, não estudar ainda:

- Tailwind
- Vue
- Angular
- Docker avançado
- Kubernetes
- Microserviços
- GraphQL
- Redis
- AWS avançado

Primeiro dominar:

```text
Python + Django + Bootstrap + PostgreSQL + React
```