# Desafio IMTS

Desafio de admissão 2019.2 IMTS - Eventilândia.


## Início

Essas instruções farão com que você tenha uma visão de como será a avaliação. Repare bem as obrigatoriedades que o processo exigirá e os bônus que estarão disponíveis para aumentar a sua pontuação
nesse teste.

A avaliação se dará através da análise da construção de um Servidor Flask (utilizando qualquer versão, a partir da 3, da linguagem de programação Python). 

Boas práticas de programação, desenvolvimento de padrões de projetos e controle de versão serão habilidades obrigatórias para esse desafio. Essas skills serão responsáveis por 0.6 da avaliação.

Implementações de outras habilidades: migrações e versionamento de banco de dados, emprego de ORM - Object Relational Mapper, controle de acesso às rotas do Servidor, utilização de um banco de dados em memória - Redis (implementação de alguma forma de cache, p.e.) e integração com outras API (e-mail, p.e.) serão skills responsáveis pelo resto da composição da nota: 0.4.

O Servidor, basicamente, deverá ser responsável pelo controle de Eventos e seus respectivos Usuários. 

Usuários devem poder se inscrever à Eventos, desde que estes estejam dentro do intervalo de inscrição do Evento. Eventos devem possuir dois intervalos: o de inscrição e o ao qual ele estará ocorrendo. Listar, editar, salvar e deletar serão funcionalidades obrigatórias para os dois modelos. Autenticar e redefinir senha exclusivos ao segundo, Usuários. A autenticação deve retornar um token JWT

Todos os modelos devem ter a capacidade de serem persistidos em um Banco de Dados relacional, [Postgresql](https://www.postgresql.org/), possuindo, assim, um identificador único universal, uma chave primária. Essa deve possuir 36 caracteres (dica, [uuid](https://pt.wikipedia.org/wiki/Identificador_%C3%BAnico_universal)). 

O modelo de Usuários deve possuir, além do identificador universal, os seguintes atributos: nome, username, password, telefone, aniversário e e-mail.

Já o modelo de Eventos deve ter, também além do indentificador universal: título, descrição, data início, data fim, data início inscrições, data fim inscrições.

A funcionalidade de inscrição de Usuários à Eventos pode ser realizada tanto com uma tabela adicional, p.e. UsuarioEvento, relacionando os dois modelos, quanto com um atributo array no modelo adequado. Esta funcionalidade fica sob responsabilidade do desafiado (rsrsrs).


### Instalação

Uma estrutura básica, com algumas dependências, estará disponível. Sinta-se com liberdade para editar essa
arquitetura.

Algumas dependências, à nível de auxílio, estarão presentes no `requirements.txt`. Para fazer a instalação dessas dependências, aconselho a utilização de alguma biblioteca para virtualização de ambientes (p.e. conda ou virtualenv). Para instalar as dependências, execute, p.e.:

```
pip3 install -r requirements.txt
```

Feito
```
until finished
```

End with an example of getting some data out of the system or using it for a little demo

## Running the tests

Explain how to run the automated tests for this system

### Break down into end to end tests

Explain what these tests test and why

```
Give an example
```

### And coding style tests

Explain what these tests test and why

```
Give an example
```

## Deployment

Add additional notes about how to deploy this on a live system


## Authors

* **Billie Thompson** - *Initial work* - [PurpleBooth](https://github.com/PurpleBooth)

See also the list of [contributors](https://github.com/your/project/contributors) who participated in this project.


## Acknowledgments

* Hat tip to anyone whose code was used
* Inspiration
* etc

