## Um simples CRUD em Nodejs e Mysql

### Clonando e instalando projeto
Copie e cole em seu terminal
```bash
git clone https://github.com/HugoBCuri/crud-nodejs-mysql.git
```

Entre na pasta
```bash
cd crud-nodejs-mysql
```

Baixe e instale os pacotes do projeto
```bash
npm install
```

### Criando a base de dados
Entre no MySQL pelo terminal
```bash
mysql -u root -p
```

Crie a base e a tabela
```sql
-- creating database
CREATE DATABASE crudnodejsmysql;

-- to use database
use crudnodejsmysql;

-- creating a new table
CREATE TABLE customer (
  id INT(6) UNSIGNED AUTO_INCREMENT PRIMARY KEY,
  name VARCHAR(50) NOT NULL,
  address VARCHAR(100) NOT NULL,
  phone VARCHAR(15)
);
```
saia do seu MySQL
```bash
exit
```

### Rodando o projeto
Para rodar basta
```bash
node src/app.js
```
Agora basta entrar na página

- [localhost:8080](http://localhost:8080)
