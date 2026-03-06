# Prática – Modelo de Processo Iterativo Incremental

## Objetivo da prática
Aplicar o modelo Iterativo Incremental em um projeto simples, passando por:
* Levantamento inicial de requisitos
* Definição de incrementos
* Planejamento de iterações
* Entrega evolutiva do sistema

---

## Tema sugerido
Sistema Web de Questionários Acadêmicos

* Criar questionários
* Cadastrar perguntas
* Aplicar escala Likert (0 a 5 )
* Registrar respostas
* Gerar relatório simples

---

## O que precisamos definir primeiro?
* **Cliente:** Coordenador de curso
* **Problema:** Ele aplica questionários manualmente (Google Forms)
e depois precisa organizar dados manualmente para análise estatística. 
Ele quer um sistema próprio da instituição.

## Requisitos
Requisitos funcionais iniciais essenciais para a PRIMEIRA VERSÃO do sistema?
(Importante: pense como modelo incremental — não precisa tudo agora, só o mínimo viável.)
* Cadastro de perguntas
* Criação de um questionário
* Aplicação manual (sem login de aluno ainda)
* Relatório simples em tabela

Mesmo sem usuários cadastrados ainda, já resolve parte do problema

---

## Incremento 1
Entregar um sistema funcional capaz de:
* Cadastrar perguntas
* Criar questionário
* Registrar respostas
* Gerar relatório estatístico simples 
* Sem login
* Sem controle de aluno
* Sem perfis de usuário
* Sem permissões

### Iteratições
Podemos adicionar novas funcionalidades
Podemos melhorar o que já foi feito
Podemos refatorar estrutura
Podemos corrigir problemas descobertos

---

## Incremento 2
* Cadastro de usuários
* Controle de perfil (admin / coordenador)
* Opção de questionário anônimo ou identificado
* Relatório por usuário

### Iteração
Pergunta obrigatória/opcional
Melhorar layout
Ajustar relatório
Melhorar desempenho
Melhorar interface

---
#### Se no Incremento 1 o cliente disser:
“Gostei, mas preciso que as perguntas possam ser obrigatórias ou opcionais.”
R: Iteração sobre o incremento atual

#### Suponha que após o Incremento 1 o cliente diga:
“Agora preciso que apenas usuários logados possam criar questionários.” 
R: Novo incremento

#### Qual é o maior risco de tentar colocar login já no Incremento 1?
R: “Podemos fazer trabalho desnecessário caso o questionário seja anônimo.”

---

O modelo iterativo incremental não é só sobre dividir funcionalidades.
Ele é uma estratégia de:
* Redução de risco
* Entrega contínua de valor
* Validação progressiva de requisitos
* Controle de complexidade