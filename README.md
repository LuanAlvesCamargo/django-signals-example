# Django Signals Example

Este projeto demonstra a implementação prática de signals no Django, apresentando um caso de uso real para rastreamento automático de histórico de registros.

## 📋 Sobre o Projeto

O projeto implementa um sistema simples de cadastro de pessoas com um mecanismo automático de histórico utilizando Django signals. Cada vez que uma pessoa é cadastrada ou atualizada, um registro histórico é automaticamente criado.

## 🚀 Funcionalidades

- Cadastro de pessoas com nome, email e telefone
- Histórico automático de alterações usando Django signals
- Interface administrativa para gerenciamento de registros
- Demonstração prática do uso de signals no Django

## 💻 Tecnologias Utilizadas

- Python
- Django 3.2.8
- SQLite

## 🛠️ Estrutura do Projeto

```
django-signals-example/
  ├── django_signals/      # Configurações principais do projeto
  └── sinais/             # Aplicativo principal
      ├── models.py       # Definição dos modelos (Pessoa e Histórico)
      ├── signals.py      # Implementação dos signals
      └── admin.py        # Configuração da interface administrativa
```

## 📦 Modelos

### Pessoa

- Nome
- Email
- Telefone

### Histórico

- Nome
- Email
- Telefone
- Referência à Pessoa

## 🔧 Como Instalar

1. Clone o repositório

```bash
git clone https://github.com/LuanAlvesCamargo/django-signals-example.git
cd django-signals-example
```

2. Crie um ambiente virtual

```bash
python -m venv venv
source venv/bin/activate  # Linux/Mac
# ou
venv\Scripts\activate     # Windows
```

3. Instale as dependências

```bash
pip install django==3.2.8
```

4. Execute as migrações

```bash
python manage.py migrate
```

5. Crie um superusuário

```bash
python manage.py createsuperuser
```

6. Inicie o servidor

```bash
python manage.py runserver
```

## 🔍 Como Usar

1. Acesse o admin do Django em `http://localhost:8000/admin`
2. Faça login com as credenciais do superusuário
3. Adicione ou edite registros de pessoas
4. Observe como o histórico é automaticamente criado/atualizado

## 🤝 Contribuindo

Contribuições são bem-vindas! Sinta-se à vontade para:

1. Fazer um fork do projeto
2. Criar uma branch para sua feature (`git checkout -b feature/AmazingFeature`)
3. Commit suas mudanças (`git commit -m 'Add some AmazingFeature'`)
4. Push para a branch (`git push origin feature/AmazingFeature`)
5. Abrir um Pull Request

## ✨ Agradecimentos

- Django Framework
- Comunidade Python/Django
