# Isabela_2bim_MercadoTangerinasFelizes
# 🍊 Mercado Tangerinas Felizes

## Sobre o projeto

O Mercado Tangerinas Felizes é um sistema desenvolvido para a disciplina de Desenvolvimento Web 1 (DW1).

O objetivo do projeto é simular um pequeno mercado, permitindo que o usuário consulte informações dos produtos cadastrados no banco de dados.

A página foi desenvolvida utilizando HTML, CSS e JavaScript. Já o servidor foi desenvolvido em Node.js utilizando o framework Express. Os dados ficam armazenados em um banco de dados PostgreSQL.

---

# Como o projeto funciona

Quando o usuário abre a página, ele encontra algumas opções de consulta.

Ele pode:

- Ver todos os produtos cadastrados;
- Ver todas as categorias;
- Ver os produtos separados por categoria;
- Pesquisar um produto pelo nome;
- Pesquisar produtos escolhendo uma categoria e uma faixa de preço.

Sempre que o usuário clica em um botão ou faz uma pesquisa, o JavaScript envia uma requisição para o servidor.

O servidor recebe essa requisição, consulta o banco de dados PostgreSQL e procura as informações solicitadas.

Depois disso, o servidor envia a resposta em formato JSON para o navegador.

Por fim, o JavaScript recebe essas informações e mostra o resultado na própria página.

---

# Tecnologias utilizadas

- HTML5
- CSS3
- JavaScript
- Node.js
- Express
- PostgreSQL
- Biblioteca pg
- Dotenv

---

# Arquivos do projeto

**mercado.html**

Contém toda a estrutura da página.

**style.css**

Responsável pelo visual da página, como cores, imagens, botões e organização dos elementos.

**script.js**

Realiza as requisições ao servidor utilizando a Fetch API e mostra os resultados na tela.

**server.js**

Cria o servidor, recebe as requisições do navegador, consulta o banco de dados e envia as respostas.

**banco_dados.sql**

Possui os comandos para criar as tabelas e inserir os registros no banco de dados.

**package.json**

Guarda as dependências utilizadas no projeto.

**.gitignore**

Impede que arquivos e pastas desnecessárias, como `node_modules` e `.env`, sejam enviados para o GitHub.

---

# Como executar o projeto

### 1. Instale as dependências

```bash
npm install
```

### 2. Configure o arquivo .env

Crie um arquivo chamado **.env** com as informações de conexão do banco de dados.

Exemplo:

```env
DB_HOST=localhost
DB_PORT=5432
DB_NAME=SeuBanco
DB_USER=postgres
DB_PASSWORD=SuaSenha
PORT=3001
```

### 3. Crie o banco de dados

Execute o arquivo **banco_dados.sql** utilizando o PGAdmin 4 ou DBeaver.

### 4. Inicie o servidor

```bash
node server.js
```

O servidor será iniciado em:

```
http://localhost:3001
```

### 5. Abra a página

Abra o arquivo **mercado.html** no navegador.

---

# Fluxo do projeto

O funcionamento do sistema acontece da seguinte forma:

**Usuário → Página HTML → JavaScript → Servidor Node.js → Banco de Dados PostgreSQL → Servidor → JavaScript → Página HTML**

Ou seja:

1. O usuário faz uma consulta.
2. O JavaScript envia a requisição para o servidor.
3. O servidor consulta o banco de dados.
4. O banco devolve as informações.
5. O servidor envia os dados em JSON.
6. O JavaScript recebe esses dados e mostra o resultado na página.

---

# Desenvolvido por

**Isabela Maria Ferreira dos Santos**

Projeto desenvolvido para a disciplina de Desenvolvimento Web 1 (DW1) - 2º Bimestre.
