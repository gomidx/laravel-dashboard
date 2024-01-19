# Projeto de cadastro de vendas e cálculo de comissões

Esse projeto consiste em um dashboard de vendas e vendedores. Suas funcionalidades são:

1. Cadastro, login e logout de usuários adiministradores
2. Listagem, cadastro, edição e exclusão de vendedores
3. Envio de um relatório por e-mail das vendas do dia e suas respectivas comissões ao vendedor
4. Listagem e cadastro de vendas
5. Envio de um relatório por e-mail para o administrador logado de todas as vendas do dia
6. Envio diário às 18h de um relatório por e-mail para os vendedores de todas suas vendas e respectivas comissões do dia
7. Autenticação para acessar o dashboard

Na pasta /api contém a API do projeto desenvolvida em Laravel, e na pasta /dashboard contém o frontend do projeto desenvolvido também em Laravel.

## 🚀 Setup do projeto

### 🔧 Inicialização

Para começarmos, é necessário inicializar os containers da API primeiramente, executando os seguintes comandos na raíz do projeto:

```
cd api && sudo make run-api
```

Após os containers serem iniciados, a API pode ser acessada através da URL http://localhost:8000.

Agora precisamos iniciar os containers do frontend executando os seguintes comandos na raíz do projeto:

```
cd dashboard && sudo make run-web
```

Agora é só esperar os containers serem iniciados e pronto! Será possível acessar o dashboard através da URL http://localhost:8001.

## ⚙️ Testes

Para executar os testes da API, execute os seguintes comandos na raíz do projeto:

```
cd api && sudo make run-api-tests
```

### 🔧 Finalização

Para finalizar o projeto por completo, é necessário finalizar todos os containers que foram iniciados.

Para finalizar os containers da API, execute o seguinte comando na raíz do projeto:

```
cd api && sudo make kill-api
```

Para finalizar os containers do frontend, execute o seguinte comando na raíz do projeto:

```
cd dashboard && sudo make kill-web
```

Obs.: caso apresente algum erro na primeira inicialização, finalize a aplicação e a inicie novamente.

## 🛠️ Construído com

* [PHP](https://www.php.net/)
* [Laravel](https://laravel.com/)
* [Docker](https://www.docker.com/)

---
Desenvolvido com ❤️ e muito ☕ por [Lucas Gomide](https://github.com/gomidx)