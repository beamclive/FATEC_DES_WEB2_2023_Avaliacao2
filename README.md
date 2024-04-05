# Segundo Desafio Técnico da matéria de Desenvolvimento Web 2
Este projeto em PHP tem a finalidade de controlar os acessos de alunos que poderão fazer uso do estacionamento da Fatec Araras. 

### Tecnologias: 
PHP Estruturado e SGBD MySQL.

### Campos utilizados no cadastro: 

- Nome Completo
- Placa do Carro ou Moto <br><br>
  
Assim que cadastrados, os vigilantes poderão verificar os registros de entrada e saída

O desafio técnico é dar manutenção no sistema contido na pasta portarias.

### Requisitos atingidos: 

- DashBoard - Área de login/logout com uso de sessões (sessions)

Login: fatec <br>
Senha: portaria

Ao acessar index.php via POST, se a superglobal $_POST['nome'] for 'fatec' e a superglobal $_POST['senha'] for 'portaria', é setado a superglobal $_SESSION['online'] com o valor True
e a superglobal $_SESSION['username'] com o valor "Portaria Fatec", redirecionando para a página principal.php

- Verificar Veículos
Verificar somente em uma sessão ativa. Ao tentar cadastrar em uma sessão desativada, é redirecionado para a área de login.

Na primeira página (registros.php), uma caixa de seleção (combobox) com todas as placas cadastradas será apresentada.

Ao selecionar uma placa de clicar no botão Acessar, a página (registros_encontrados.php) apresenta todos os registros cadastrados na tabela registro.

Acessando a página registros_encontrados.php via GET, é redirecionado para a página registros.php.

- Cadastrar novas placas
  
Em uma sessão ativa, é possível cadastrar na tabela veículos um novo registro, com o nome completo e a placa do veículo.

Ao acessar a página cadastro_placa.php via GET, é redirecionado para a página cadastro.php.


