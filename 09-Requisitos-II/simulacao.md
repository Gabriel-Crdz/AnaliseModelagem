# Engenharia de Requisitos II

## Elicitação de Requisitos 
**SIMULAÇÃO:**

**Cliente:** "Eu tenho um hotel pequeno e preciso organizar melhor minhas reservas e hóspedes"

**Analista:** "Quais dados precisa armazenar em uma reserva?"

* Pergunta bem direcionada.
    - Focada em uma entidade (reserva) e pediu dados específicos.
    - Você está focando só em dados, ainda não em ações.

**Cliente:** "Olha, na reserva eu preciso do nome do hóspede, data de entrada, data de saída, número do quarto e a forma de pagamento."

* Indícios de requisitos funcionais:
    - associar hóspede à reserva 
    - definir datas (entrada/saída) 
    - vincular quarto 
    - registrar pagamento

**Analista:** "uma reserva pode ser cancelada? Se sim com quantos dias de antecedência?" 

* Saiu de “dados” e foi para:
    - regra de negócio 
    - comportamento do sistema 
    - condições (antecedência)

**Cliente:** "Sim, pode cancelar. Mas tem que ser com pelo menos 2 dias de antecedência, senão cobra uma diária."

* Requisitos funcionais:
    - cancelar reserva 
    - calcular cobrança em caso de cancelamento fora do prazo 
* Regra de negócio (importantíssimo):
    - cancelamento permitido até 2 dias antes 
    - após isso = cobrança de 1 diária

**Analista:** "O sistema será um APP que funciona apenas em celular ou um sistema online responsivo?"

**Cliente:** ""Prefiro que seja um sistema online, que eu possa acessar pelo navegador, tanto no computador quanto no celular."

* RNF (usabilidade / portabilidade):
    - sistema deve ser acessível via navegador 
    - deve funcionar em desktop e mobile


## Exercicio
Com base em tudo que você levantou até agora, me diga:
* Liste do sistema de hotel:
    - 5 requisitos funcionais 
    - 2 requisitos não funcionais 

* Regras:
    - escreva como requisito (não só ideia solta) 
    - use verbos claros 
    - nada genérico

### Requisitos Funcionais (RF)
* **RF01 – Gerenciamento de hóspedes**
    - O sistema deve permitir cadastrar, editar, excluir e consultar hóspedes, armazenando informações como nome, endereço, data de nascimento e contato.

* **RF02 – Gerenciamento de reservas**
    - O sistema deve permitir criar, editar, consultar e cancelar reservas, associando hóspedes a quartos e definindo datas de entrada e saída.

* **RF03 – Associação de reserva**
    - O sistema deve vincular cada reserva a um hóspede e a um quarto disponível.

* **RF04 – Gerenciamento de quartos**
    - O sistema deve permitir cadastrar, editar, excluir e consultar quartos, incluindo número, tipo e valor da diária.

* **RF05 – Consulta de disponibilidade**
    - O sistema deve permitir consultar a disponibilidade de quartos com base nas datas de entrada e saída informadas.

### Requisitos Não Funcionais (RNF)
* **RNF01 – Desempenho**
O sistema deve apresentar a lista de quartos disponíveis em até 3 segundos para 95% das requisições.

* **RNF02 – Acessibilidade e responsividade**
O sistema deve ser acessível via navegador web e possuir interface responsiva, permitindo uso em dispositivos desktop e móveis.