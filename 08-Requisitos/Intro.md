# Engenharia de Requisitos

**Requisitos:** Definir o que o sistema desse fazer

* **Funcionais:** O que o sistema faz, age. Ex: Login, Cadastro.
* **Não-Funcionais:** Qualidade do sistema, melhoria de um requisito funcional. EX: Segurança, Desempenho.

## Por que sistemas falham?
R: Requisitos **MAL DEFINIDOS**

Ex:
1. "O sistema deve ser rapido"
2. "O sistema deve ser facil de usar"
3. "Quero que o sistema deva ter uma interface moderna"

Reescrevendo(Detalhando para melhorar o requisito):

1. "O sistema deve responder as requisições do usuario em até 3 segundos"
2. "O sistema deve permitir que um usuario realize o cadastro de um aluno em no maximo 2 min."
3. "O sistema deve possuir interface dinamica, compativel com multiplataformas(Web, Mobile)."


## Requisitos Funcionais X Não Funcionais

Exercicio:

Qualifique cada requisito como: RF, RNF, e justifique:

1. O sistema deve permitir que o usuário realize login 
    * RF, descreve uma ação que o usuario precisa fazer

2. O sistema deve responder às requisições em até 3 segundos
    * RNF, descreve um comportamento de resposta

3. O sistema deve gerar relatório de vendas mensal 
    * RF, descreve uma função de relatorio

4. O sistema deve ser fácil de usar 
    * RNF, e um comportamento, 
    e está muito genérico melhor seria "“Usuário deve conseguir realizar X em até Y passos”" 

5. O sistema deve permitir pagamento via cartão de crédito 
    * RF, uma função de uma regra de negocios

6. O sistema deve estar disponível 99% do tempo 
    * RNF, um comportamento, não diz o que ele faz, mas como ele deve fazer 

7. O sistema deve permitir cadastro de produtos 
    * RF, uma funcionalidade basica do sistema

8. O sistema deve garantir a segurança dos dados dos usuários
    * RNF, comportamento de segurança dos dados, NÃO descreve uma funcionalidade específica 

### PARA NUNCA MAIS ERRAR
**RF = ação clara do sistema (verbo funcional)**
- cadastrar 
- gerar 
- permitir 
- calcular 

Não necessariamente mensurável com números, mas precisa ser sem ambiguidade

* **Ruim:** O sistema deve gerenciar reservas
* **Melhor:** O sistema deve permitir criar, editar, cancelar e visualizar reservas de quartos

**RNF = qualidade, restrição ou critério**
- rápido 
- seguro 
- disponível 
- usável

* **Ruim:** O sistema deve ser rápido
* **Melhor:** O sistema deve responder em até 2 segundos

### TORNANDO REQUISITOS MELHORES 
Transforme os requisitos abaixo em versões boas e mensuráveis:

**O sistema deve ser rápido:**
* O sistema deve responder às requisições de busca em até 3 segundos para 95% das requisições simultânea de até 100 usuários 

**O sistema deve ser seguro:** 
* O sistema deve bloquear o usuário após 3 tentativas consecutivas de login inválido por 5 minutos 

**O sistema deve ser fácil de usar:**
* Um usuário iniciante deve conseguir realizar o cadastro em até 3 minutos sem auxílio externo 

**O sistema deve ter boa performance:** 
* O sistema deve permitir que operações demoradas não bloqueiem a interface por mais de 1 segundo 