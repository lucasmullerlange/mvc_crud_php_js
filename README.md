

O Projeto foi desenvolvido em javascript CSS e Boostrap para validação de formluário e php e mysql no Back-End 

<i> Baixe o xampp : </i>

    https://www.apachefriends.org/pt_br/index.html
    instale o xampp depois de baixado em sua pasta de downloads

<i> Depois de instalado, dentro do xampp click em : </i>
    
    
    Através do terminal no (mac ou linux) e no powershe(windows)

     Localize a pasta chamada  "htdocs"
    
<i> Clone o repositório dentro da pasta htdocs: </i>

    git clone https://github.com/lucasmullerlange/crud_clients_mvc 

Rodando dentro da pasta htdocs e dando start no xampp
    no navegador digite : 

    http://localhost/crud-mvc-php/index.php

 <i> 2 - Configurando o banco  : </i>
    
<i> Conexao.class.php </i>
    definimos a senha e o user do banco MySql 

    mysql:host=localhost;dbname=agendamentos;", "root"
    No arquivo agendamentos.sql terá a query do mysql. 
    
 Obs: Eu não defini senha pois achei melhor para ganhar tempo. Mas não é uma boa prática deixar sem.

PRONTO!! Banco configurado com a aplicação 
 
        http://localhost/phpmyadmin/  
        Aqui vai direto para o MySql 

       Na opção SQL clicamos em e abrirá algo para digitar 
       Coloque isso dentro : 

        Copie aqui e cole lá 

         CREATE DATABASE agendamentos; 
        USE agendamentos;
        CREATE TABLE registros (
        `id` int(11) NOT NULL AUTO_INCREMENT,
        `name` varchar(100) NOT NULL,
        `email` varchar(100) NOT NULL,
        `cpf` varchar(50) NOT NULL,
        `birth` date NOT NULL,
        `address` varchar(100) NOT NULL,
        `phone` varchar(50) NOT NULL,
        PRIMARY KEY(id)
        );

        INSERT INTO `registros` (`id`, `name`, `email`, `cpf`, `birth`, `address`, `phone`) VALUES
        (01, 'Teste', 'teste@teste.com', '123.456.789-00', '2020-01-31', 'rua teste', '(00) 0000-0000');


Lá no lado direto click em executar ... Banco executado ... 






     


       