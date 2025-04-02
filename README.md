# 😄 Piadas App

<div align="center">
  <img src="https://img.shields.io/badge/python-3.8+-blue.svg" alt="Python 3.8+">
  <img src="https://img.shields.io/badge/flask-3.0.2-green.svg" alt="Flask 3.0.2">
  <img src="https://img.shields.io/badge/license-MIT-yellow.svg" alt="License MIT">
</div>

Uma aplicação web divertida para compartilhar piadas, com sistema de cadastro e aprovação de usuários. Desenvolvida com Flask e Bootstrap para uma experiência moderna e responsiva.

## ✨ Funcionalidades

- 👤 Sistema de cadastro e login de usuários
- 🔒 Sistema de aprovação de novos usuários por administradores
- 📝 Compartilhamento de piadas com título e conteúdo
- 📱 Interface moderna e responsiva
- 🎨 Design limpo e intuitivo com Bootstrap 5
- 🔐 Autenticação segura com Flask-Login

## 🚀 Tecnologias Utilizadas

- Python 3.8+
- Flask 3.0.2
- Flask-SQLAlchemy
- Flask-Login
- Flask-WTF
- Bootstrap 5
- SQLite (banco de dados)

## 📋 Pré-requisitos

Antes de começar, você precisa ter instalado em sua máquina:
- Python 3.8 ou superior
- pip (gerenciador de pacotes Python)
- Git (opcional, para clonar o repositório)

## 🛠️ Instalação e Configuração

### 1. Clonando o Repositório

```bash
# Clone o repositório
git clone https://github.com/acaciomartins/piadas_app.git

# Entre no diretório do projeto
cd piadas_app
```

### 2. Criando o Ambiente Virtual

```bash
# Crie um ambiente virtual
python -m venv venv

# Ative o ambiente virtual
# No Windows:
venv\Scripts\activate
# No Linux/Mac:
source venv/bin/activate
```

### 3. Instalando as Dependências

```bash
# Instale as dependências do projeto
pip install -r requirements.txt
```

### 4. Criando o Usuário Administrador

```bash
# Execute o script para criar o usuário admin
python create_admin.py
```

### 5. Iniciando a Aplicação

```bash
# Execute a aplicação
python run.py
```

A aplicação estará disponível em `http://localhost:5000`

## 👑 Credenciais do Administrador

Após executar o script `create_admin.py`, você terá acesso ao painel administrativo com as seguintes credenciais:

- Email: admin@example.com
- Senha: admin123

## 📖 Como Usar a Aplicação

### Para Usuários Comuns

1. Acesse a aplicação em `http://localhost:5000`
2. Clique em "Registrar" para criar uma nova conta
3. Preencha o formulário de registro com seus dados
4. Aguarde a aprovação do administrador
5. Após aprovado, você poderá fazer login e compartilhar piadas

### Para Administradores

1. Faça login com as credenciais de administrador
2. Acesse o painel administrativo
3. Na seção "Usuários Pendentes de Aprovação", você verá a lista de novos usuários
4. Clique em "Aprovar" para autorizar um usuário a compartilhar piadas

## 🏗️ Estrutura do Projeto

```
piadas_app/
├── app/
│   ├── __init__.py
│   ├── models.py
│   ├── routes/
│   │   ├── main.py
│   │   ├── auth.py
│   │   └── admin.py
│   ├── forms.py
│   └── templates/
│       ├── base.html
│       ├── index.html
│       ├── login.html
│       ├── register.html
│       ├── nova_piada.html
│       └── admin/
│           └── dashboard.html
├── config.py
├── create_admin.py
├── run.py
└── requirements.txt
```

## 🤝 Contribuindo

Contribuições são sempre bem-vindas! Sinta-se à vontade para:

1. Fazer um fork do projeto
2. Criar uma branch para sua feature (`git checkout -b feature/AmazingFeature`)
3. Commit suas mudanças (`git commit -m "Add some AmazingFeature"`)
4. Push para a branch (`git push origin feature/AmazingFeature`)
5. Abrir um Pull Request

## 📝 Licença

Este projeto está sob a licença MIT. Veja o arquivo [LICENSE](LICENSE) para mais detalhes.

## 👥 Autores

- Acacio Martins - [@acaciomartins](https://github.com/acaciomartins)

## 🙏 Agradecimentos

- Flask Team
- Bootstrap Team
- Todos os contribuidores do projeto
