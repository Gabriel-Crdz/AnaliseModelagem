# Atividade Avaliativa III

## Sistema de Gestão da Copa do Mundo

### Objetivo

Desenvolver o diagrama de classes de um Sistema de Gestão da Copa do Mundo utilizando a linguagem UML e a ferramenta PlantUML.

O objetivo do sistema é permitir o gerenciamento completo de uma competição internacional de futebol, contemplando informações sobre seleções, jogadores, partidas, estádios, grupos da competição e demais elementos envolvidos na organização do torneio.


### Cenário

A Federação Internacional de Futebol pretende informatizar o gerenciamento da Copa do Mundo. O sistema deverá armazenar informações sobre as seleções participantes, seus jogadores, os grupos da competição, os estádios utilizados e as partidas realizadas durante o torneio.

Cada seleção possui informações próprias, como nome, sigla, ranking internacional, técnico responsável e continente ao qual pertence. Além disso, cada seleção é formada por diversos jogadores.

Os jogadores possuem dados cadastrais, posição em campo, número da camisa e estatísticas individuais. Durante a competição, eles participam das partidas representando suas respectivas seleções.

A competição é organizada em grupos. Cada grupo recebe uma identificação e reúne diversas seleções que disputam vagas para as fases eliminatórias.

As partidas acontecem em estádios específicos. Cada estádio possui informações como nome, cidade, capacidade de público e data de inauguração.

Para cada partida é necessário registrar a data, horário, fase da competição, seleções participantes, placar final e estádio onde o jogo ocorreu.

O sistema também deverá permitir a existência de diferentes tipos de pessoas relacionadas ao evento. Por exemplo, jogadores e técnicos possuem características em comum, mas também apresentam informações específicas de suas funções.

Além disso, cada partida gera registros estatísticos, como posse de bola, quantidade de finalizações, cartões e faltas cometidas pelas equipes participantes.

### Requisitos de Modelagem

O diagrama de classes deverá atender aos seguintes requisitos:
* Utilizar obrigatoriamente a ferramenta PlantUML.
* Conter no mínimo 7 classes.
* Cada classe deverá possuir:
    - No mínimo 5 atributos;
    - No mínimo 3 métodos.
* O modelo deverá conter obrigatoriamente:
    - Pelo menos uma relação de herança;
    - Pelo menos uma relação de agregação;
    - Pelo menos uma relação de composição;
    - Associações com multiplicidades adequadas.
* Devem ser identificadas corretamente as responsabilidades de cada classe.
* Os atributos devem possuir tipos de dados adequados.
* Os métodos devem representar comportamentos coerentes com o domínio do problema.
