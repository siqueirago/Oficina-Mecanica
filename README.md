# Projeto de Banco de Dados - Oficina Mecânica

## Descrição do Projeto
Projeto desenvolvido como parte de um desafio para criação de um esquema conceitual para uma oficina mecânica.
O banco de dados foi projetado para atender às necessidades operacionais da oficina, permitindo o registro de clientes, veículos, mecânicos, serviços, peças e ordens de serviço (OS).
O modelo é capaz de organizar os dados de forma estruturada, facilitando o controle de informações e a geração de relatórios.

## Objetivo
Este projeto tem como objetivo criar um esquema conceitual de banco de dados para o controle e gerenciamento de execução de ordens de serviço em uma oficina mecânica,  com base na narrativa fornecida

## Narrativa

* Sistema de controle e gerenciamento de execução de ordens de serviço em uma oficina mecânica
* Clientes levam veículos à oficina mecânica para serem consertados ou para passarem por revisões  periódicas
* Cada veículo é designado a uma equipe de mecânicos que identifica os serviços a serem executados e preenche uma OS com data de entrega.
* A partir da OS, calcula-se o valor de cada serviço, consultando-se uma tabela de referência de mão-de-obra
* O valor de cada peça também irá compor a OSO cliente autoriza a execução dos serviços
* A mesma equipe avalia e executa os serviços
* Os mecânicos possuem código, nome, endereço e especialidade
* Cada OS possui: n°, data de emissão, um valor, status e uma data para conclusão dos trabalhos.

## Modelo Conceitual
###  Diagrama entidade-relacionamento

![oficina](https://github.com/user-attachments/assets/4128e479-d410-46db-8f71-b9e3e696cfde)


###  Relacionamentos

* Cliente possui Veículo (1:N)

* Veículo está associado a Ordem de Serviço (1:N)

* Ordem de Serviço inclui Serviços (N:M)

* Ordem de Serviço inclui Peças (N:M)

* Equipe é composta por Mecânicos (1:N)

* Equipe executa Ordem de Serviço (1:N)

## Ferramentas Utilizadas

* Ferramenta de Modelagem: MySQL Workbench para criar o diagrama de entidade-relacionamento (ER).

* Linguagem de Banco de Dados: SQL (para futuras implementações físicas).


## Observações
Se você quiser contribuir para este projeto, siga estes passos:

* Fork este repositório
* Crie um novo branch
* Faça suas alterações
* Crie um pull request

## Autor
* Julio Siqueira
* Siqueiragomes75@gmail.com
* (85) 981304584

