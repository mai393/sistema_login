# Sistema Login PHP

## Recursos

* Cadastro de usuários
* Login e Logout
* Perfil do usuário
* Alteração de e-mail
* Alteração de senha
* Upload de foto de perfil
* Sistema de anotações
* Proteção contra SQL Injection
* Senhas criptografadas com `password_hash()`
* Página inicial (`index.php`)
* Compatível com hospedagem InfinityFree

## Tecnologias

* PHP procedural com templates inline/PHP “mixed with HTML”
* MySQL
* Bootstrap 5.3.3
* PDO

## Como executar localmente

1. Importe o banco de dados `sistema_login.sql`.
2. Configure as credenciais em `includes/conexao.php`.
3. Inicie o Apache e o MySQL.
4. Acesse:

```text
http://localhost/sistema_login/
```

## Hospedagem no InfinityFree

1. Crie uma conta no InfinityFree.
2. Crie um banco de dados MySQL no painel.
3. Importe o arquivo `sistema_login.sql`.
4. Atualize as credenciais em `includes/conexao.php`.
5. Envie todos os arquivos para a pasta `htdocs`.
6. Acesse o domínio fornecido pelo InfinityFree.

## Usuário de teste

E-mail: [caio@gmail.com](mailto:caio@gmail.com)

Senha: (utilize a senha cadastrada no banco)

## Estrutura do Projeto

```text
index.php
login.php
cadastro.php
dashboard.php
profile.php
notes.php

includes/
 ├─ conexao.php
 ├─ auth.php

uploads/
```

## Segurança

* Prepared Statements com PDO
* Proteção contra SQL Injection
* Senhas armazenadas com `password_hash()`
* Verificação de sessão para páginas protegidas
