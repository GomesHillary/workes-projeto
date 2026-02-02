# WorkES — Plataforma de Busca de Prestadores de Serviço

O **WorkES** é um projeto inspirado no conceito de um “iFood de prestadores de serviços”, conectando clientes e profissionais em um único lugar.

![img.png](img.png)
![img_3.png](img_3.png)
![img_1.png](img_1.png)
![img_2.png](img_2.png)
![img_4.png](img_4.png)
A aplicação permite:

- Buscar serviços (ex.: eletricista, encanador, pintor etc.)
- Cadastrar prestadores
- Editar serviços já cadastrados
- Criar conta, fazer login e logout
- Navegação simples e responsiva

---

## Tecnologias Utilizadas

### Backend
- Python 3
- Flask
- Flask-Login
- Flask-Bcrypt
- Flask-SQLAlchemy
- SQLite

### Frontend
- HTML5
- CSS3
- JavaScript puro

### Templates
- Jinja2

---

## Funcionalidades

### Busca de Serviços
Sistema de busca baseado em:
- Nome do serviço
- Local
- Descrição

As requisições são feitas via AJAX (JSON) para o endpoint `/buscar`.

---

### Autenticação de Usuários
- Cadastro com e-mail e senha
- Senhas criptografadas com Bcrypt
- Login seguro
- Rotas protegidas por `@login_required`

---

### Cadastro de Prestadores
Usuários autenticados podem registrar:
- Nome do serviço
- Local
- Telefone (opcional)
- Link externo (site, Instagram, WhatsApp etc.)
- Descrição

Os dados são armazenados em SQLite.

---

### Edição de Serviços
Permite edição de serviços pela rota:

`/editar/<id>`# WorkES — Plataforma de Busca de Prestadores de Serviço


### Edição de Serviços
Permite edição de serviços pela rota:

`/editar/<id>`
