# Projeto de Login e Registro de Contas

Este projeto é uma aplicação web simples que oferece funcionalidades de login, registro de contas e um painel de administração especial para gerenciar contas.

## Requisitos

Certifique-se de ter os seguintes requisitos instalados:

- Node.js
- MySQL Server (a versão deve estar dentro de 5.6 and 8.0.35)
- MySQL Workbench
- Express
- Express Sessions
- MySQL for Node.js

Para instalar as dependências, utilize o comando:

```bash
npm install
```

## Configuração do Banco de Dados

Execute o arquivo "nodelogin.sql" no MySQL Workbench. Este arquivo SQL contém uma conta de membro e uma conta de administrador que podem ser usadas para fins de teste.

Certifique-se de que o servidor MySQL esteja rodando na porta 3306.

## Iniciar o Servidor

Para iniciar o servidor, utilize o comando:

```bash
npm run start
```

Se tudo estiver configurado corretamente, acesse **http://localhost:3000/** no seu navegador. Isso o levará ao formulário de login.

## Variáveis 

Configure suas variáveis de ambiente criando um arquivo `.env` na raiz do projeto e inclua as seguintes linhas:

```env
DB_HOST = localhost
DB_USER = seu_usuario // default: "root"
DB_PASSWORD = sua_senha_aqui
```

## Funcionalidades

**Login e Registro:** Os usuários podem se autenticar ou registrar novas contas.

**Painel de Administração:** Se autenticado como administrador, o usuário terá acesso a uma aba especial para gerenciar contas.

### Acesso para Administrador
- Username: admin
- Password: admin

### Acesso para Membro
- Username: member
- Password: member


## Importante!

⚠️ **Observação:** Tive alguns problemas de compatibilidade com a versão v21.1.0 do node, caso tenha o mesmo problema utilize a versão, utilize o nvm e faça downgrade do node para a versão v20.9.0