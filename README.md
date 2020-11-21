# api-cadastra-pessoas
Api utilizada para treinamento de testes de API, construída com base em tutorial da treinaweb e adaptada para necessidade das aulas, para mais informações sobre a API original acesse  https://www.treinaweb.com.br/blog/criando-uma-api-rest-com-o-spring-boot/


Roteiro para startar e usar a API localmente 

1-  Faça download do software xampp e execute o instalador (next next next finish)
https://www.apachefriends.org/pt_br/download.html

2- Faça clone ou download deste projeto


3- Acesse o xamp control panel e clique em start em apache, em mysql
-> Apache gerencia tanto o mysql quando o toncat
-> MYSQL é um banco de dados que é acessível através da ferramenta PHPMYADmim


4- Acessar http://localhost/phpmyadmin/ e criar uma nova base dados com o nome apirest

5- Executar a classe DemoApplication

6- Abra o seu navegador e acesse http://localhost:8080/pessoa , deverá ter um retorno vazio porque o banco de dados ainda não tem nada

5- Acesse novamente http://localhost/phpmyadmin/ clique em apirest (banco que você criou) e execute o seguinte script

INSERT INTO `pessoa` (`id`, `cpf`, `nome`, `telefone`) VALUES
(0, '02137984748', 'Aline Zanin', '998885777'),
(1, '02137984748', 'Maria Aparecida Zilva', '99262728272'),
(2, '02137984748', 'Carmem Souza', '99371117188'),
(3, '02137984748', 'Joana Carla', '996373637'),
(4, '02137984748', 'Pedro Silva', '97735536278'),
(5, '02137984748', 'João Silva', '997665343'),
(6, '02137984748', 'Avelino Pedroso', '9977733777'),
(7, '02137984748', 'Amanda Silveira', '9928827827'),
(8, '02137984748', 'Carlos Pereira', '997227789'),
(9, '02137984748', 'Daniele Silveira', '9977766272'),
(10, '02137984748', 'Amanda Loureiro', '991229283'),
(11, '02137984748', 'Joana Clarinda Gomes', '999999999'),
(12, '02137984748', 'Paulo Ferreirra', '998887788'),
(13, '02137984748', 'Julio Lima', '9887664545'),
(14, '02137984748', 'Juliana Freitas', '998776447');


Para saber mais sobre esta api que vamos utilizar acesse este tutorial, ela foi extraida dele https://www.treinaweb.com.br/blog/criando-uma-api-rest-com-o-spring-boot/
