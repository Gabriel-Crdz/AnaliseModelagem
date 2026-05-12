# Pratica Metodologias Ageis

O cliente pediu:
“Uma escola precisa de um sistema simples.”

## Product Backlog
"Criem o product backlog"
"Liste pelo menos 5 funcionalidades (1 item = 1 funcionalidade)"

1. Cadastrar usuarios
2. Registro de presença do aluno
3. Mural onde pode-se colocar avisos e tarefas
4. Criar turmas e associar alunos e professores
5. Login

---

## Sprint

### Backlog

**PRIORIZAÇÃO:** “Agora vocês não podem fazer tudo.”
“Escolham 3 funcionalidades MAIS IMPORTANTES para a primeira Sprint”

* Cadastro de aluno
* Login
* Registro de frequencia

### Estimativa de tempo (Story Points)

“Estimar o esforço de cada tarefa.”
Usem apenas esses valores:
**1 (fácil), 2 (médio), 3 (difícil), 5 (muito difícil)**

1. Registro de frequencia (1)
2. Cadastro de aluno (2)
3. Login (3)

### Rodada 1

Regras:
* Máximo 2 tarefas em ‘Fazendo’
* Só pode mover se estiver trabalhando

**Quadro**
| A fazer | Fazendo | Feito |
|---------|---------|-------|
| Frequencia | Cadastro | |
| | Login | |
| | | |

#### Evento Inesperado

“O login parou de funcionar!”

**SITUAÇÃO**
A tarefa Login agora tem problema
Vocês precisam decidir o que fazer

**Perguntas:**

1. Vocês param tudo ou continuam?
    * Param tudo: Foco total no bug.

2. O que fazem com a tarefa de login?
    * **Swarm** - todo mundo ajuda no login.

3. O que acontece com as outras tarefas?
    * Ficam em pausa, ou voltam para "A fazer".

R: "No Scrum, quando a um problema, tudo para e a priorridade é corrigir o erro".

### Rodada 2

Continuação do bug: “O bug AINDA não foi resolvido.”

**Quadro**
| A fazer | Fazendo | Feito |
|---------|---------|-------|
| Frequencia | Login | |
| Cadastro | | |
| | | |

**Resultado da rodada 2:** Não foi imediato(Rodada 1), mas reagiram bem e corrigiram rapido o problema.

### Rodada 3

“O sistema voltou a funcionar.”

**Quadro**
| A fazer | Fazendo | Feito |
|---------|---------|-------|
| | Cadastro | Login |
| | Frequencia | |
| | | |

### Rodada 4

“Vocês continuam trabalhando…”
“O cadastro de alunos é mais difícil do que parecia!”

**IMPACTO:** A tarefa “Cadastro de Alunos” ficou mais pesada
Vai demorar mais do que o esperado

**Quadro**
| A fazer | Fazendo | Feito |
|---------|---------|-------|
| Frequencia | Cadastro | Login |
| | | |
| | | |

“A equipe está focada no cadastro de alunos…”

### Rodada 5

“O cadastro de alunos foi concluída”

**Quadro**
| A fazer | Fazendo | Feito |
|---------|---------|-------|
| | Frequencia | Login |
| | | Cadastro |
| | | |

**TESTE FALHOU:** “O registro de frequência não passou no teste!”

**IMPACTO:** a tarefa NÃO pode ir para “Feito”
Precisa voltar e ser corrigida

### Rodada 6

**Quadro**
| A fazer | Fazendo | Feito |
|---------|---------|-------|
| | Frequencia | Login |
| | | Cadastro |
| | | |

O cliente não aprovou a frequencia, então ela continua no "Fazendo".

### Rodada 7

**Quadro**
| A fazer | Fazendo | Feito |
|---------|---------|-------|
| | | Login |
| | | Cadastro |
| | | Frequencia |

A frequencia foi concluida a tempo, mesmo com problemas

---

## Kanban

"O cliente gostou do sistema, mas agora quer melhorias contínuas.”

“Não teremos mais Sprint fechada.”

“Agora vocês trabalham em fluxo contínuo (Kanban)”

“O sistema precisa evoluir.”

### Novo backlog:
* Recuperação de senha
* Relatório de presença
* Cadastro de professores
* Notificações
* Edição de cadastro

### NOVAS REGRAS

Regras do Kanban:

Máximo 2 tarefas em ‘Fazendo’

Máximo 1 tarefa em ‘Teste’

Não pode pular etapas

**Quadro:** [ Backlog ] | [ A Fazer ] | [ Fazendo ] | [ Teste ] | [ Feito ]

Ex:
| Backlog | A fazer | Fazendo | Teste | Feito |
|---|---|---|---|---|
| Rec. Senha | Cad. Prof | Rel. Presença | Rec. Senha | |
| Rel. Presença | Notificações | | | |
| Cad. Prof | Edt. Cadastro | | | |
| Notificação | | | | | |
| Edt. Cadastro | | | | | |

**ENSINAMENTO CHAVE:** “Em Kanban, o objetivo não é começar tarefas… **É terminar tarefas**"

* **Scrum:** "Trabalho por pacotes fechados de tempo" -> **PARALELO**
* **Kanban:** "Trabalho como uma fila" -> **SERIAL**