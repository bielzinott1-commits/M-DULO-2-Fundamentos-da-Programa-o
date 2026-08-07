# CURSO COMPLETO DE PROGRAMAÇÃO

# Do Zero ao Desenvolvedor Full Stack

## Volume 2 – Fundamentos da Programação

# CAPÍTULO 12

# Algoritmos, Fluxogramas e Pseudocódigo: Planejando Programas Antes de Codificar

> **Objetivo do capítulo:** Ao final deste capítulo, você será capaz de criar algoritmos organizados, desenhar fluxogramas profissionais e escrever pseudocódigos para transformar ideias em soluções antes de utilizar uma linguagem de programação.

---

# Introdução

Um dos maiores erros de programadores iniciantes é começar escrevendo código sem pensar na solução.

Exemplo:

A pessoa abre o editor e começa:

```javascript
let x = "";
```

Mas ela ainda não sabe:

* quais dados precisa receber;
* quais decisões o programa deve tomar;
* qual resultado deseja entregar.

Programadores profissionais seguem uma regra:

> Primeiro resolva o problema. Depois escreva o código.

Para isso existem três ferramentas fundamentais:

1. **Algoritmos**
2. **Fluxogramas**
3. **Pseudocódigo**

---

# 1. O que é um algoritmo?

Um algoritmo é uma sequência finita de passos organizados para resolver um problema.

Características de um algoritmo:

## Entrada

São os dados recebidos.

Exemplo:

```text
Nome do usuário
Senha
Idade
```

---

## Processamento

São as ações realizadas.

Exemplo:

```text
Verificar senha

Calcular idade

Realizar operação
```

---

## Saída

É o resultado.

Exemplo:

```text
Login realizado

Resultado do cálculo

Mensagem de erro
```

---

# Exemplo simples de algoritmo

Problema:

> Fazer um programa que calcule a soma de dois números.

Algoritmo:

```
Início

1. Receber primeiro número.

2. Receber segundo número.

3. Somar os dois números.

4. Mostrar resultado.

Fim.
```

---

# Características de um bom algoritmo

Um algoritmo deve ser:

## Claro

Qualquer pessoa deve entender.

---

## Organizado

Os passos devem estar em ordem.

---

## Finito

Deve possuir um fim.

---

## Preciso

Cada etapa deve indicar exatamente o que fazer.

---

# Algoritmo no cotidiano

## Exemplo: Fazer café

```
Início

Pegar uma xícara.

Colocar café.

Adicionar açúcar.

Adicionar água quente.

Misturar.

Servir.

Fim.
```

Observe:

Mesmo sem programação, existe lógica.

---

# 2. O que é um fluxograma?

Um fluxograma é uma representação visual de um algoritmo.

Ele utiliza símbolos para mostrar o caminho que o programa seguirá.

É muito usado em:

* desenvolvimento de software;
* engenharia;
* empresas;
* planejamento de sistemas.

---

# Por que usar fluxogramas?

Eles ajudam a:

* visualizar problemas;
* encontrar erros;
* explicar sistemas;
* planejar programas.

---

# Principais símbolos de fluxograma

## 1. Início/Fim

Formato:

```
( Oval )
```

Representa:

* começo;
* término.

Exemplo:

```
( Início )
```

---

# 2. Processo

Formato:

```
[ Retângulo ]
```

Representa uma ação.

Exemplo:

```
[ Calcular média ]
```

---

# 3. Entrada/Saída

Formato:

```
/ Paralelogramo /
```

Representa informações recebidas ou exibidas.

Exemplo:

```
/ Digitar nome /
```

---

# 4. Decisão

Formato:

```
◇ Losango ◇
```

Representa uma pergunta.

Exemplo:

```
    ◇
Senha correta?
```

Possíveis caminhos:

```
Sim → entrar

Não → erro
```

---

# 5. Linha de fluxo

Representada por setas.

Exemplo:

```
Início

 ↓

Processo

 ↓

Fim
```

---

# Exemplo de fluxograma

Problema:

Verificar se uma pessoa é maior de idade.

Fluxograma:

```
        (Início)

            ↓

     / Digitar idade /

            ↓

     [ Ler idade ]

            ↓

        ◇ Idade >=18? ◇

        ↓              ↓

      Sim             Não

       ↓               ↓

[ Maior idade ]  [ Menor idade ]

        \          /

            ↓

          (Fim)
```

---

# 3. O que é pseudocódigo?

Pseudocódigo é uma forma de escrever algoritmos utilizando uma linguagem parecida com programação, mas mais simples.

Ele não pertence a nenhuma linguagem específica.

Serve para planejar.

---

# Exemplo

Problema:

Somar dois números.

Pseudocódigo:

```
INÍCIO

Ler número1

Ler número2

resultado ← número1 + número2

Mostrar resultado

FIM
```

---

# Pseudocódigo x Código real

## Pseudocódigo:

```
Ler idade

Se idade >= 18

Mostrar maior idade

Senão

Mostrar menor idade
```

---

## JavaScript:

```javascript
let idade = 20;

if(idade >= 18){

console.log("Maior idade");

}else{

console.log("Menor idade");

}
```

---

# Estrutura básica de um algoritmo

Todo algoritmo geralmente possui:

```
INÍCIO

Entrada de dados

Processamento

Saída

FIM
```

---

# Variáveis no pseudocódigo

Variáveis armazenam informações.

Exemplo:

```
nome ← "Davi"

idade ← 15
```

Em programação:

```javascript
let nome = "Davi";

let idade = 15;
```

---

# Operadores matemáticos

Usados para cálculos.

| Operador | Significado      |
| -------- | ---------------- |
| +        | Soma             |
| -        | Subtração        |
| *        | Multiplicação    |
| /        | Divisão          |
| %        | Resto da divisão |

---

# Exemplo:

```
numero1 ← 10

numero2 ← 5

resultado ← numero1 + numero2

Mostrar resultado
```

Saída:

```
15
```

---

# Estruturas de decisão

Decisões permitem que o programa escolha caminhos.

Exemplo:

```
SE condição

FAÇA algo

SENÃO

FAÇA outra coisa
```

---

# Exemplo:

Sistema de aprovação escolar:

```
INÍCIO

Ler nota

SE nota >= 7

Mostrar "Aprovado"

SENÃO

Mostrar "Reprovado"

FIM
```

---

# Estruturas de repetição

Servem para repetir ações.

Exemplo:

Mostrar números de 1 até 10.

Pseudocódigo:

```
INÍCIO

Para número de 1 até 10

Mostrar número

Fim Para

FIM
```

---

# Algoritmos com menus

Exemplo:

Sistema bancário:

```
INÍCIO

Mostrar opções:

1 - Saldo

2 - Transferência

3 - Sair


Escolher opção


Executar ação


FIM
```

---

# Como criar um algoritmo profissional

Siga estes passos:

---

## 1. Entenda o problema

Exemplo:

"Preciso criar um sistema de login."

Pergunte:

* Quem usa?
* Quais dados preciso?
* Qual resultado esperado?

---

## 2. Liste entradas

Exemplo:

```
Email

Senha
```

---

## 3. Defina processos

Exemplo:

```
Verificar usuário

Comparar senha

Autorizar acesso
```

---

## 4. Defina saídas

Exemplo:

```
Login realizado

Senha incorreta
```

---

## 5. Faça o fluxograma

Visualize a lógica.

---

## 6. Faça o pseudocódigo

Escreva a solução.

---

## 7. Transforme em código

Escolha a linguagem.

---

# Exemplo completo: Sistema de login

## Problema:

Criar login.

---

## Algoritmo:

```
Início

Receber email

Receber senha

Buscar usuário no banco

Comparar dados

Se estiver correto

Liberar acesso

Senão

Mostrar erro

Fim
```

---

## Fluxograma:

```
(Início)

 ↓

Entrada email/senha

 ↓

Buscar usuário

 ↓

◇ Dados corretos? ◇

 ↓             ↓

Sim           Não

 ↓             ↓

Acesso       Erro

 ↓

(Fim)
```

---

## Pseudocódigo:

```
INÍCIO

LER email

LER senha


SE email e senha estiverem corretos

    MOSTRAR "Login aprovado"

SENÃO

    MOSTRAR "Dados inválidos"


FIM
```

---

# Ferramentas para criar fluxogramas

Algumas ferramentas utilizadas:

* Draw.io
* Lucidchart
* Microsoft Visio
* Canva
* Figma

---

# Erros comuns de iniciantes

❌ Começar pelo código.

❌ Não planejar.

❌ Misturar etapas.

❌ Criar algoritmos sem fim.

❌ Ignorar possibilidades de erro.

---

# Exercícios

1. Explique o que é um algoritmo.
2. Qual a diferença entre algoritmo e fluxograma?
3. Para que serve o pseudocódigo?
4. Quais são os três elementos principais de um programa?
5. Crie um algoritmo para preparar uma refeição.
6. Crie um fluxograma para verificar senha.
7. Escreva um pseudocódigo para calcular média escolar.
8. Explique o símbolo de decisão em um fluxograma.
9. Por que programadores planejam antes de codificar?
10. Transforme um algoritmo simples em código JavaScript.

---

# Projeto Prático

Crie um planejamento completo para um:

# Sistema de Cadastro de Usuários

Faça:

## 1. Algoritmo

Incluindo:

* entrada;
* processamento;
* saída.

---

## 2. Fluxograma

Mostrando:

* início;
* cadastro;
* validação;
* resultado.

---

## 3. Pseudocódigo

Com:

* variáveis;
* decisões;
* mensagens.

---

Depois transforme esse planejamento em um programa utilizando uma linguagem de programação.

---

# Resumo do capítulo

Neste capítulo você aprendeu:

✅ O que são algoritmos.
✅ Como criar soluções passo a passo.
✅ O conceito de fluxograma.
✅ Símbolos utilizados profissionalmente.
✅ O que é pseudocódigo.
✅ Entrada, processamento e saída.
✅ Decisões e repetições.
✅ Como planejar sistemas antes de programar.

---

## Próximo capítulo

No **Capítulo 13**, você aprenderá **Variáveis, Tipos de Dados e Operadores**, entrando oficialmente na programação prática. Você entenderá como os computadores armazenam informações, como manipular dados e como criar os primeiros programas reais.
