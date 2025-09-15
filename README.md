# CRUD de Livros em Laravel

Este é o projeto final para a disciplina de Introdução a Laravel, consistindo em um sistema de Gerenciamento, Leitura, Atualização e Deleção (CRUD) para uma entidade de Livros.

## [cite_start]O que foi implementado [cite: 36]

O projeto cumpre com todos os requisitos obrigatórios solicitados:

* [cite_start]**Autenticação Ativa:** O CRUD é exclusivo para usuários autenticados[cite: 18].
* [cite_start]**Rotas Resource:** Utiliza o padrão de rotas `resource` do Laravel para todas as operações do CRUD (`index`, `create`, `store`, `edit`, `update`, `destroy`)[cite: 19].
* [cite_start]**Validação no Servidor:** Os formulários de criação e edição possuem validação server-side para garantir a integridade dos dados[cite: 20].
* [cite_start]**Mensagens de Sessão (Flash):** O sistema exibe mensagens de sucesso após a criação, atualização ou exclusão de um registro[cite: 21].
* [cite_start]**Views Limpas:** As telas foram desenvolvidas com HTML e CSS personalizados para uma interface simples e legível[cite: 22].
* [cite_start]**Tratamento de "Estado Vazio":** A página de listagem exibe uma mensagem específica quando nenhum livro está cadastrado[cite: 23].

## [cite_start]Como Instalar e Rodar [cite: 34]

Siga os passos abaixo para executar o projeto em um ambiente local.

1.  **Clone o repositório:**
    ```bash
    git clone [https://url-do-seu-repositorio.git](https://url-do-seu-repositorio.git)
    cd nome-do-projeto
    ```

2.  **Instale as dependências do PHP:**
    ```bash
    composer install
    ```

3.  **Configure o arquivo de ambiente:**
    ```bash
    cp .env.example .env
    ```

4.  **Gere a chave da aplicação:**
    ```bash
    php artisan key:generate
    ```

5.  **Configure o banco de dados** no arquivo `.env` com suas credenciais locais.
    ```env
    DB_CONNECTION=mysql
    DB_HOST=127.0.0.1
    DB_PORT=3306
    DB_DATABASE=laravel
    DB_USERNAME=root
    DB_PASSWORD=
    ```

6.  **Execute as migrações** para criar as tabelas no banco de dados:
    ```bash
    php artisan migrate
    ```

7.  **Instale as dependências do front-end:**
    ```bash
    npm install
    ```

8.  **Compile os assets e inicie o watcher:**
    ```bash
    npm run dev
    ```

9.  **Inicie o servidor local** (em um novo terminal):
    ```bash
    php artisan serve
    ```

A aplicação estará disponível em `http://127.0.0.1:8000`.

## Usuário de Teste

[cite_start]Ao executar o projeto em um ambiente local, o banco de dados será criado do zero e a tabela de usuários estará vazia.

Para testar as funcionalidades que exigem autenticação, por favor, **crie um novo usuário** através da página de registro, disponível em `/register`.
