# Configurando MySQL

Baixar e configurar o MySQL e MySQL Workbrench

~~~sql
create database teste;

use teste;

create table usuario (
id int not null auto_increment,
nome varchar(255) not null,
email varchar(255) not null,
fone varchar(45) not null,
data_nascimento date not null,
primary key (id)
);

insert into usuario (nome, email, fone, data_nascimento)
values ('helder', 'helder@helder.com', '98065-7337', '1989-12-17');
~~~

Configurando o MySQL para trabalhar localmente
~~~sql
alter user 'root'@'localhost' identified with mysql_native_password by '123456';
~~~

# Criando o Ambiente backend com Node.js
~~~bash
// inicializando o projeto node.js
npm init -y

// instalando as bibliotecas necessárias
npm install express nodemon mysql cors
~~~

## Inicializando o programa e visualizando os retornos

```js
npm start
// acessar o localhost com qualquer navegador
localhost:8800

// essa porta é indicado no código index.js no projeto de api
```

# Criando o App React

```js
npx create-react-app ./

// instalando as bibliotecas necessárias
npm install styled-components axios react-icons react-toastify
```