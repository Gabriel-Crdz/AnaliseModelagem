# Documentos de Caso de Uso

Esse documento **transforma o desenho em especificação textual** do sistema.
Normalmente ele é usado para:

* explicar exatamente o comportamento do sistema 
* orientar programadores 
* orientar testes
* validar regras com o cliente
* servir de documentação oficial do software

### Um diagrama mostra:
* atores 
* casos 
* relacionamentos

**Mas ele NÃO explica:**
* o que acontece primeiro
* o que o usuário digita
* o que o sistema responde
* erros e exceções

O **documento textual** resolve isso.

### No diagrama existe:

**Caso de Uso: “Realizar Login”**

Mas o documento detalha:
* usuário informa login 
* sistema valida 
* sistema pede senha 
* sistema verifica 
* sistema libera acesso
* se senha estiver errada = mostra erro.

---
## Ficha de Documentação

| Campos | Função |
|--------|--------|
| Nome | Nome do caso de uso |
| Objetivo | O que ele faz |
| Atores | Quem participa |
| Pré-condições | O que precisa existir antes |
| Pós-condições | O que fica pronto depois |
| Fluxo Principal | Caminho normal |
| Fluxos Alternativos | Caminhos Opcionais |
| Fluxos de Exceções | Erros/Problemas |
| Regras de Negócio | Restrições Importantes |

### Exemplo
**Sistema:** Sistema de controle de vendas
**Caso de Uso:** Realizar venda

A primeira coisa importante é entender: “Qual problema esse caso de uso resolve?”

O objetivo NÃO é explicar o passo a passo ainda. É apenas resumir a finalidade do caso de uso.

**Exemplo ruim:**

“O usuário clica no botão vender.”

Isso é ação/interface.

**Exemplo bom:**

“Permitir que uma venda seja registrada 

**Regra importante**

Em documentos de caso de uso, normalmente evitamos:
* frases muito longas 
* explicações detalhadas; 
* mencionar interface (“clicar no botão”); 
* escrever “o sistema deve”. 

Escreva frases objetivas no infinitivo:
* Permitir cadastro... 
* Registrar venda... 
* Consultar cliente... 
* Emitir relatório... 

| Campos | Conteúdo |
|--------|----------|
| Sistema | Sistema de Controle de Vendas |
| Caso de Uso | Realizar venda |
| Objetivo | Permitir o registro de vendas no sistema |

### Atores

Identificar:

Quem participa desse caso de uso?

No diagrama provavelmente tem um ator ligado ao caso “Realizar Venda”.

R: Vendedor

### Pré-condições

Agora começamos a entrar na lógica do sistema.

Pré-condição significa:

O que precisa ser verdade **ANTES** do caso de uso começar?

Ou seja: Sem isso, a venda não pode acontecer.

| Pré-condição | Motivo |
|------|-------|
| Produto cadastrado | Não é possivel vender algo inexistente |
| Vendedor autenticado | O sistema precisa saber <br> quem está realizado a venda |

### Pós-condições

O que deve ser verdade DEPOIS que o caso de uso termina com sucesso?

Ou seja: Qual estado o sistema ficou após concluir a venda?

**Exemplos possíveis**
* venda registrada 
* estoque atualizado

### Fluxo Principal
O caminho feliz do caso de uso.

Ou seja:
* tudo dá certo 
* sem erros 
* sem exceções 
* sem caminhos alternativos

**Exemplo simplificado**
1. Vendedor inicia venda. 
2. Sistema solicita produtos. 
3. Vendedor informa produtos. 
4. Sistema calcula total. 
5. Vendedor informa pagamento. 
6. Sistema registra venda. 
7. Sistema atualiza estoque. 
8. Sistema finaliza venda.

**Regra  importante**
* usar verbos de ação
* mostrar interação ator ↔ sistema
* seguir ordem cronológica
* ter passos numerados

| Passo | Descrição |
|-------|-----------|
| 01 | Vendedor inicia a venda |
| 02 | Sistema solicita os itens da venda |
| 03 | Vendedor informa os itens da venda |
| 04 | Sistema calcula o valor total da venda |
| 05 | Vendedor informa o tipo de pagamento |
| 06 | Vendedor registra o pagamento |
| 07 | Sistema a venda |
| 08 | Sistema atualiza o estoque de produtos |
| 09 | Sistema atualiza o caixa |
| 10 | Sistema finaliza a venda |

### Fluxos Alternativos

um caminho diferente, MAS ainda válido.

Ou seja: não é erro

**o caso continua funcionando.**

**Exemplos em vendas**
* pagamento em cartão 
* pagamento parcelado 
* venda com desconto 
* venda sem cliente cadastrado
* Tudo isso pode ser alternativo

### Fluxo de Exceção
situações em que o objetivo do caso de uso não consegue continuar normalmente.
* erro
* bloqueio
* inconsistência
* falha
* cancelamento

No passo 3 do fluxo principal:

Vendedor informa um produto. 

Sistema verifica que o produto não está cadastrado. 

Sistema exibe mensagem de erro. 

Sistema solicita que outro produto seja informado.

### Regra de Negócio
É uma regra que o sistema é obrigado a respeitar.
* restrições
* limites
* políticas da empresa
* condições obrigatórias

**Exemplo:**

“Descontos acima de 10% exigem autorização.”

“Não é permitido vender produto sem estoque.”

“O caixa deve estar aberto para registrar vendas.”

“A venda deve possuir ao menos um item.”

| Regra | Tipo |
|-------|------|
| estoque não pode ficar negativo | restrição |
| desconto maximo de 15% | limite |
| venda exige pagamento | obrigatoriedade |
| apenas gerente cancela venda | permissão |