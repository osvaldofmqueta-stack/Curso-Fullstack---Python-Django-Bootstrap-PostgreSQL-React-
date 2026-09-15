# Curso Fullstack — Python, Django, Bootstrap, PostgreSQL e React

Este curso segue uma progressão única: começa em **Python, lógica e programação**, passa pelos fundamentos da web e só avança para Django quando a base estiver consolidada.

## Objetivo final

No fim do curso, serás capaz de criar, testar e publicar uma aplicação full-stack com:

```text
React + Bootstrap → Django REST Framework → PostgreSQL
```

Também saberás criar aplicações completas apenas com:

```text
Django Templates + Bootstrap + PostgreSQL
```

## Stack principal

- **Python** — lógica, programação e backend
- **HTML** — estrutura das páginas
- **CSS** — fundamentos visuais
- **Bootstrap** — estilização rápida e responsiva
- **JavaScript** — interatividade no navegador
- **Django** — aplicações web e backend
- **SQLite** — primeira base de dados
- **PostgreSQL** — base de dados profissional
- **Django REST Framework** — APIs
- **React** — frontend moderno
- **Git e GitHub** — versões e portfólio
- **pytest** — testes

Bootstrap será o framework visual principal. Tailwind, Vue, Angular e outras tecnologias ficam para depois.

# Ritmo de estudo

- 5 dias por semana
- 2 horas por dia
- 10 horas por semana
- 28 semanas
- Aproximadamente 280 horas

## Estrutura de cada aula — 120 minutos

| Atividade | Tempo |
|---|---:|
| Revisão e correção da aula anterior | 10 min |
| Explicação do conceito | 20 min |
| Exemplo acompanhado | 35 min |
| Exercício individual | 40 min |
| Debug, resumo e commit | 15 min |
| **Total** | **120 min** |

### Organização da semana

- **Segunda:** conceito novo e exemplos
- **Terça:** exercícios guiados
- **Quarta:** exercício individual
- **Quinta:** construção do projeto
- **Sexta:** revisão, testes, documentação e GitHub

## Regra para avançar

Não avançar apenas porque as semanas terminaram. Avançar quando conseguires:

1. Explicar o conceito com as tuas palavras.
2. Criar um exercício sem copiar o exemplo.
3. Corrigir pelo menos um erro sozinho.
4. Entregar o projeto da etapa.

Cada fase abaixo tem um **ponto de passagem**. Se ainda não conseguires cumprir os critérios, repete os exercícios antes de seguir.

# Instalações por etapa

Não instalar tudo de uma vez.

## Antes da primeira aula

Instalar:

1. Google Chrome
2. Visual Studio Code
3. Python
4. Git
5. Criar uma conta GitHub

Confirmar:

```bash
python --version
git --version
```

Em alguns computadores:

```bash
python3 --version
```

## Ambiente virtual Python

Criar dentro de cada projeto Python:

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

Atualizar o pip:

```bash
python -m pip install --upgrade pip
```

## Instalações posteriores

Quando chegar a cada fase:

```bash
# Django
python -m pip install django

# Django REST Framework
python -m pip install djangorestframework

# Testes
python -m pip install pytest pytest-django
```

Para PostgreSQL, instalar PostgreSQL e pgAdmin apenas na fase de bases de dados.

Para React, instalar Node.js LTS e confirmar:

```bash
node --version
npm --version
```

# Fase 1 — Python, lógica e programação

**Semanas 1–6 · 60 horas**

Esta é a fundação do curso. Não começar Django antes de concluir esta fase.

## Semana 1 — Ambiente e sintaxe

Estudar:

- VS Code e terminal
- Variáveis
- Tipos de dados
- Strings
- Números
- `print`
- Entrada de dados
- Operadores

Exercícios:

- Apresentação do utilizador
- Calculadora
- Conversor de temperatura
- Conversor de idade

## Semana 2 — Condições e ciclos

Estudar:

- `if`
- `elif`
- `else`
- `for`
- `while`
- `range`
- Operadores lógicos

Exercícios:

- Verificar maioridade
- Verificar número par ou ímpar
- Criar uma tabuada
- Sistema de notas
- Jogo de adivinhação

## Semana 3 — Estruturas de dados

Estudar:

- Listas
- Tuplos
- Dicionários
- Conjuntos
- Índices
- Percorrer estruturas
- Compreensões de listas

Exercícios:

- Lista de compras
- Agenda de contactos
- Inventário de produtos
- Pesquisa numa lista
- Contagem de palavras

## Semana 4 — Funções e organização

Estudar:

- Criar funções
- Parâmetros
- Retorno
- Escopo
- Módulos
- Importações
- Reutilização de código

Exercícios:

- Calculadora dividida em funções
- Sistema de menu
- Funções para gerir produtos
- Funções para validar dados

## Semana 5 — Ficheiros, JSON e erros

Estudar:

- Ler ficheiros
- Escrever ficheiros
- JSON
- `try`
- `except`
- `finally`
- Erros comuns

Exercícios:

- Guardar contactos num JSON
- Ler produtos de um ficheiro
- Guardar resultados de um jogo
- Validar entradas inválidas

## Semana 6 — Classes e projeto Python

Estudar:

- Classes
- Objetos
- Atributos
- Métodos
- `__init__`
- Noções de programação orientada a objetos

### Projeto da fase

**Gestor financeiro no terminal**

Funcionalidades:

- Registar receitas
- Registar despesas
- Calcular saldo
- Listar movimentos
- Categorizar movimentos
- Guardar dados em JSON
- Tratar entradas inválidas

### Ponto de passagem para a web

Só avançar se conseguires:

- Criar um programa Python sem seguir cada linha de um tutorial.
- Dividir o código em funções.
- Usar listas e dicionários.
- Ler e guardar JSON.
- Corrigir erros básicos.
- Explicar a diferença entre função, classe e objeto.

# Fase 2 — Fundamentos da web

**Semanas 7–10 · 40 horas**

Python será o backend, mas precisas compreender o navegador antes de usar Django.

## Semana 7 — HTML

Estudar:

- Estrutura HTML
- Títulos e parágrafos
- Links
- Imagens
- Listas
- Tabelas
- Formulários
- Elementos semânticos

Projeto pequeno:

- Página pessoal com biografia, competências e contactos

## Semana 8 — CSS

Estudar:

- Seletores
- Cores
- Fontes
- Margens
- Espaçamentos
- Bordas
- Flexbox
- Grid
- Responsividade

Exercícios:

- Cartão de perfil
- Navbar
- Galeria
- Layout para telemóvel

## Semana 9 — Bootstrap

Bootstrap é o framework de estilização escolhido por ser simples, documentado e adequado para Django.

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

## Semana 10 — JavaScript básico no navegador

Estudar:

- Variáveis
- Funções
- Arrays
- Objetos
- DOM
- Eventos
- Validação
- `localStorage`

### Projeto da fase

**Portfólio pessoal responsivo**

- Página inicial
- Sobre mim
- Competências
- Projetos
- Contacto
- Bootstrap
- Design para computador e telemóvel

### Ponto de passagem para Django

Conseguir:

- Criar uma página HTML sem copiar a estrutura.
- Criar um formulário.
- Fazer uma página responsiva.
- Usar Flexbox ou Grid.
- Usar Bootstrap para montar cards, navbar e formulários.
- Criar uma interação simples com JavaScript.

# Fase 3 — Django e aplicações web

**Semanas 11–15 · 50 horas**

## Semana 11 — Primeiro projeto Django

Instalar:

```bash
python -m pip install django
```

Criar:

```bash
django-admin startproject config .
python manage.py startapp core
python manage.py runserver
```

Estudar:

- Projeto
- Aplicação
- Servidor
- URLs
- Views
- Templates

## Semana 12 — Templates e Bootstrap

Estudar:

- `base.html`
- Herança de templates
- Blocos
- Ficheiros estáticos
- CSS no Django
- Bootstrap no Django

Estrutura:

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

## Semana 13 — Models, migrations e Admin

Estudar:

- Models
- Campos
- Migrations
- SQLite
- Django Admin
- ORM

Comandos:

```bash
python manage.py makemigrations
python manage.py migrate
python manage.py createsuperuser
python manage.py runserver
```

## Semana 14 — Formulários e CRUD

Estudar:

- Django Forms
- ModelForms
- Validação
- Mensagens
- Criar
- Listar
- Editar
- Apagar

## Semana 15 — Projeto Django

### Projeto

**Blog pessoal com Django e Bootstrap**

- Criar artigos pelo Admin
- Listar artigos
- Ver artigo completo
- Categorias
- Pesquisa
- Formulário de contacto
- Layout responsivo

### Ponto de passagem para bases de dados e autenticação

Conseguir:

- Criar uma aplicação Django.
- Ligar URLs a views.
- Renderizar templates.
- Usar um model.
- Fazer migrations.
- Criar um CRUD.
- Usar Bootstrap dentro dos templates.

# Fase 4 — Bases de dados, autenticação e permissões

**Semanas 16–18 · 30 horas**

## Semana 16 — PostgreSQL e SQL

Instalar:

- PostgreSQL
- pgAdmin

Estudar:

- Tabelas
- Colunas
- Chaves primárias
- Relações
- SQL básico
- PostgreSQL com Django
- Migrations

## Semana 17 — Autenticação

Estudar:

- Registo
- Login
- Logout
- Sessões
- Perfil do utilizador
- Passwords

## Semana 18 — Permissões e projeto

Estudar:

- Páginas privadas
- Grupos
- Permissões
- Utilizadores comuns e administradores

### Projeto da fase

**Sistema de gestão de tarefas**

- Criar conta
- Iniciar sessão
- Criar tarefas
- Editar tarefas
- Apagar tarefas
- Marcar tarefas como concluídas
- Cada utilizador vê apenas as suas tarefas
- Interface com Bootstrap

### Ponto de passagem para APIs

Conseguir:

- Usar PostgreSQL com Django.
- Criar relações entre models.
- Implementar login e logout.
- Proteger páginas.
- Validar formulários.
- Separar permissões de utilizadores.

# Fase 5 — APIs com Django REST Framework

**Semanas 19–20 · 20 horas**

Instalar:

```bash
python -m pip install djangorestframework
```

Utilizar Thunder Client no VS Code ou Postman.

## Conteúdos

- API REST
- JSON
- Serializers
- Views de API
- ViewSets
- Routers
- GET
- POST
- PUT
- DELETE
- Autenticação e permissões em APIs

## Exercícios

- API de produtos
- API de tarefas
- API de utilizadores
- Filtros
- Pesquisa
- Endpoint protegido

### Projeto

**API de uma loja online**

Endpoints:

```text
GET    /api/produtos/
POST   /api/produtos/
PUT    /api/produtos/<id>/
DELETE /api/produtos/<id>/
```

### Ponto de passagem para React

Conseguir:

- Explicar o que é uma API.
- Criar endpoints.
- Enviar e receber JSON.
- Testar uma API.
- Proteger um endpoint.
- Ligar uma API a uma base de dados.

# Fase 6 — React e frontend moderno

**Semanas 21–23 · 30 horas**

Instalar Node.js LTS:

```bash
node --version
npm --version
```

Criar:

```bash
npm create vite@latest frontend
cd frontend
npm install
npm run dev
```

## Conteúdos

- Componentes
- JSX
- Props
- Estado
- Eventos
- Formulários
- Listas
- React Router
- `fetch`
- Comunicação com a API
- Bootstrap no React

## Exercícios

- Componente de card
- Contador
- Lista filtrável
- Formulário
- Página de login
- Navegação entre páginas

### Projeto da fase

**Dashboard React para a API Django**

- Listar produtos
- Adicionar produtos
- Editar produtos
- Apagar produtos
- Pesquisar
- Filtrar
- Fazer login
- Interface com Bootstrap

# Fase 7 — Testes, segurança e publicação

**Semanas 24–25 · 20 horas**

## Semana 24 — Testes e qualidade

Instalar:

```bash
python -m pip install pytest pytest-django
```

Estudar:

- Testes de models
- Testes de views
- Testes de APIs
- Testes de formulários
- Testes de autenticação
- Tratamento de erros

## Semana 25 — Segurança e deploy

Estudar:

- Variáveis de ambiente
- Proteção de passwords
- CSRF
- CORS
- Ficheiros estáticos
- Ficheiros de media
- Configuração de produção
- GitHub
- Deploy

### Ponto de passagem para o projeto final

Conseguir:

- Escrever testes básicos.
- Não guardar segredos no GitHub.
- Configurar variáveis de ambiente.
- Publicar uma aplicação.
- Ler logs e corrigir um erro de produção.

# Fase 8 — Projeto final full-stack

**Semanas 26–28 · 30 horas**

## Projeto recomendado

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

## Semana 26 — Planeamento e backend

- Definir o problema
- Listar funcionalidades
- Desenhar as páginas
- Criar os models
- Criar autenticação
- Criar endpoints

## Semana 27 — Frontend e integração

- Criar páginas React
- Adicionar Bootstrap
- Ligar à API
- Criar formulários
- Criar dashboard
- Mostrar estados de carregamento e erros

## Semana 28 — Qualidade e portfólio

- Testar
- Corrigir erros
- Melhorar o design
- Criar README do projeto
- Publicar
- Adicionar ao portfólio

# Resultado final

Ao concluir o curso, deverás conseguir:

- Programar em Python.
- Resolver problemas com lógica.
- Criar páginas com HTML e CSS.
- Usar Bootstrap.
- Criar interações com JavaScript.
- Construir aplicações com Django.
- Trabalhar com PostgreSQL.
- Criar login e permissões.
- Criar APIs REST.
- Criar interfaces em React.
- Escrever testes.
- Publicar aplicações.
- Apresentar projetos no GitHub.

## Tecnologias para estudar apenas depois

Não estudar no início:

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
Python → Web → Django → PostgreSQL → APIs → React → Deploy
```