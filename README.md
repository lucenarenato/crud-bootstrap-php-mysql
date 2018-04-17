# Crud Bootstrap PHP MySql
- Aqui, nós vamos utilizar o XAMPP, que já traz o PHP, o MySQL (ou MariaDB), e o phpMyAdmin para manipular o banco de dados.
- Passo 1: Crie o Banco de Dados e a Tabela de Clientes

$ Clientes (codigo, nome, cpf/cnpj, data de nascimento, 
          endereço, bairro, cep, cidade, estado, 
          telefone, celular, inscrição estadual, 
          data de cadastro, data de atualização)


- SQL, fica assim:

$ CREATE TABLE customers (	  id int(11) NOT NULL,	  name varchar(255) NOT NULL,	  cpf_cnpj varchar(14) NOT NULL,	  birthdate date NOT NULL,	  address varchar(255) NOT NULL,	  hood varchar(100) NOT NULL,	  zip_code int(8) NOT NULL,	  city varchar(100) NOT NULL,	  state varchar(100) NOT NULL,	  phone int(13) NOT NULL,	  mobile int(13) NOT NULL,	  ie int(11) NOT NULL,	  created datetime NOT NULL,	  modified datetime NOT NULL	);	
ALTER TABLE customers	  ADD PRIMARY KEY (id);	  	ALTER TABLE customers	  MODIFY id int(11) NOT NULL AUTO_INCREMENT, AUTO_INCREMENT=1;

- Se preferir, pode fazer via SQL direto (na aba SQL, do phpMyAdmin):

$ CREATE DATABASE wda_crud;

- Renato Lucena - Goiania - GO - 2018

- Quem quiser seguir essas aulas: http://webdevacademy.com.br/tutoriais/crud-bootstrap-php-mysql-parte1/