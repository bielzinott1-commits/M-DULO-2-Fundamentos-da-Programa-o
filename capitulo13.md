# CURSO COMPLETO DE PROGRAMAÇÃO

# Do Zero ao Desenvolvedor Full Stack

## Volume 2 – Fundamentos da Programação

# CAPÍTULO 13

# Variáveis, Tipos de Dados e Operadores: A Base de Todo Programa

> **Objetivo do capítulo:** Ao final deste capítulo, você entenderá como os programas armazenam informações, aprenderá o conceito de variáveis, conhecerá os principais tipos de dados e dominará os operadores utilizados para criar lógica em qualquer linguagem de programação.

---

# Introdução

Todo programa precisa trabalhar com informações.

Um aplicativo de banco precisa guardar:

* nome do cliente;
* saldo;
* senha;
* histórico de transações.

Um jogo precisa guardar:

* vida do personagem;
* pontuação;
* posição no mapa;
* itens coletados.

Mas onde essas informações ficam?

A resposta é:

# Variáveis

---

# O que é uma variável?

Uma variável é um espaço na memória do computador utilizado para armazenar um valor.

Imagine uma caixa com uma etiqueta.

Exemplo:

```text id="p7m8zy"
┌───────────────┐
│ idade         │
│ 15            │
└───────────────┘
```

A caixa é a variável.

O nome é:

```text id="t2wy7k"
idade
```

O valor armazenado é:

```text id="e2x0mh"
15
```

---

# Variáveis na programação

Exemplo em JavaScript:

```javascript id="1wy9fz"
let idade = 15;
```

Significa:

* criar uma variável chamada `idade`;
* armazenar o valor `15`.

---

# Por que variáveis são importantes?

Sem variáveis, os programas não conseguiriam lembrar informações.

Exemplo:

Sem variável:

```javascript id="q8o4mv"
console.log(15);
```

O programa apenas mostra um número.

---

Com variável:

```javascript id="5m0gk4"
let idade = 15;

console.log(idade);
```

Agora o programa sabe que aquele número representa uma idade.

---

# Como funciona a memória?

O computador possui memória RAM.

Quando você cria uma variável:

```javascript id="5e3zv2"
let nome = "Davi";
```

O computador reserva um espaço:

```text id="4v4z5t"
Memória

Endereço 1001

Valor: Davi

Nome: nome
```

---

# Declaração de variáveis

Cada linguagem possui sua própria forma.

---

# JavaScript

```javascript id="pq8nyx"
let nome = "Carlos";
```

---

# Python

```python id="w3omq8"
nome = "Carlos"
```

---

# Java

```java id="l6f8jb"
String nome = "Carlos";
```

---

# C#

```csharp id="4d9jvf"
string nome = "Carlos";
```

---

# Regras para nomes de variáveis

Um bom nome deve ser:

## Claro

Ruim:

```javascript id="9txs0g"
let x = 15;
```

Bom:

```javascript id="t7z2s0"
let idadeUsuario = 15;
```

---

## Sem espaços

Errado:

```text id="57mz1w"
nome usuario
```

Correto:

```text id="tq3y4m"
nomeUsuario
```

---

## Não começar com números

Errado:

```text id="v5j8xn"
1nome
```

Correto:

```text id="1h8n3k"
nome1
```

---

# Padrão camelCase

Muito usado em JavaScript.

Exemplo:

```javascript id="w91m3j"
nomeCompleto

dataNascimento

quantidadeProdutos
```

A primeira palavra começa minúscula e as próximas começam com letra maiúscula.

---

# Constantes

Uma constante é um valor que não pode ser alterado.

Exemplo:

```javascript id="qv8y2b"
const PI = 3.14;
```

O valor permanece igual.

---

# Variável x Constante

| Variável          | Constante     |
| ----------------- | ------------- |
| Pode mudar        | Não muda      |
| let               | const         |
| Dados temporários | Valores fixos |

---

# Exemplo:

Variável:

```javascript id="0c5hjm"
let pontos = 0;

pontos = 100;
```

A alteração é permitida.

---

Constante:

```javascript id="03ojpg"
const CPF = "123456789";
```

Não deve ser alterada.

---

# Tipos de dados

Os computadores precisam saber que tipo de informação está sendo armazenada.

Os principais tipos são:

---

# 1. String

Representa textos.

Exemplo:

```javascript id="p4rf9v"
let nome = "Davi";
```

Valores de texto ficam entre aspas.

Exemplos:

```text id="0tmn0v"
"Olá"

"Programação"

"GitHub"
```

---

# 2. Number

Representa números.

Exemplo:

```javascript id="x9u7sw"
let idade = 15;

let preco = 29.90;
```

Pode ser:

* inteiro;
* decimal.

---

# 3. Boolean

Representa verdadeiro ou falso.

Possui dois valores:

```text id="xw7l1d"
true

false
```

Exemplo:

```javascript id="4m3t9b"
let usuarioLogado = true;
```

---

# 4. Array

Lista de valores.

Exemplo:

```javascript id="c0j8hx"
let frutas = [
"maçã",
"banana",
"uva"
];
```

Um array guarda vários dados.

---

# 5. Object

Representa um objeto com informações.

Exemplo:

```javascript id="k2n1qa"
let usuario = {

nome:"Davi",

idade:15,

cidade:"Araquari"

};
```

---

# 6. Null

Representa ausência intencional de valor.

Exemplo:

```javascript id="6dq5j7"
let resultado = null;
```

Significa:

"não possui valor atualmente".

---

# 7. Undefined

Quando algo ainda não recebeu valor.

Exemplo:

```javascript id="q7c5z0"
let telefone;
```

Resultado:

```text id="5m7m9j"
undefined
```

---

# Tipagem de dados

Existem dois grandes modelos.

---

# Linguagens de tipagem dinâmica

O tipo é definido automaticamente.

Exemplo JavaScript:

```javascript id="4r7ymd"
let valor = 10;

valor = "texto";
```

Permitido.

---

# Linguagens de tipagem estática

O tipo precisa ser declarado.

Exemplo Java:

```java id="1pmqzj"
int idade = 15;
```

Não pode receber texto.

---

# Operadores

Operadores são símbolos que realizam ações.

Eles são divididos em:

* matemáticos;
* comparação;
* lógicos;
* atribuição.

---

# Operadores matemáticos

## Soma (+)

```javascript id="8tw5jr"
10 + 5
```

Resultado:

```text id="u6l4m0"
15
```

---

## Subtração (-)

```javascript id="8x4z4v"
10 - 5
```

Resultado:

```text id="g8zq20"
5
```

---

## Multiplicação (*)

```javascript id="2shk20"
10 * 5
```

Resultado:

```text id="e7j8wb"
50
```

---

## Divisão (/)

```javascript id="z9q0e5"
10 / 2
```

Resultado:

```text id="ip4z3x"
5
```

---

## Resto (%)

Retorna o restante da divisão.

Exemplo:

```javascript id="r9b6mo"
10 % 3
```

Resultado:

```text id="2y4i0j"
1
```

---

# Operadores de atribuição

Servem para colocar valores.

---

## Igual (=)

```javascript id="n9o2qa"
let idade = 15;
```

---

## Adição (+=)

```javascript id="w8j0s6"
pontos += 10;
```

É igual a:

```javascript id="1h4j79"
pontos = pontos + 10;
```

---

## Subtração (-=)

```javascript id="42hj8c"
saldo -= 50;
```

---

# Operadores de comparação

Eles retornam:

true ou false.

---

## Igualdade

```javascript id="q5h4uy"
5 == 5
```

Resultado:

```text id="69h4sa"
true
```

---

## Diferente

```javascript id="d9x0pm"
5 != 10
```

Resultado:

```text id="x4a1f7"
true
```

---

## Maior que

```javascript id="1d6w1b"
10 > 5
```

---

## Menor que

```javascript id="3n4j6m"
5 < 10
```

---

## Maior ou igual

```javascript id="b1z8fo"
idade >= 18
```

---

# Operadores lógicos

Usados para combinar condições.

---

# AND (E)

Símbolo:

```text id="l5g0i7"
&&
```

As duas condições precisam ser verdadeiras.

Exemplo:

```javascript id="n0z9h3"
idade >=18 && possuiDocumento
```

---

# OR (OU)

Símbolo:

```text id="1q3s8c"
||
```

Uma condição verdadeira já basta.

Exemplo:

```javascript id="x0f8u5"
temCartao || temPix
```

---

# NOT (NÃO)

Símbolo:

```text id="m2w7vb"
!
```

Inverte o valor.

Exemplo:

```javascript id="3r0t8m"
!logado
```

---

# Exemplo completo

Sistema de compra:

```javascript id="d4m8yn"
let saldo = 100;

let preco = 50;

let compraPermitida = saldo >= preco;

console.log(compraPermitida);
```

Resultado:

```text id="6q7n3a"
true
```

---

# Conversão de tipos

Às vezes precisamos transformar dados.

Exemplo:

Texto:

```javascript id="k8v1mr"
"10"
```

Número:

```javascript id="r7z3mf"
10
```

Conversão:

```javascript id="6u3n0v"
Number("10");
```

---

# Entrada de dados

Um programa geralmente recebe informações.

Exemplo JavaScript:

```javascript id="6gr8so"
prompt("Digite seu nome");
```

Usuário:

```text id="o5x4cv"
Davi
```

Programa:

```text id="7q9n8h"
Olá Davi
```

---

# Saída de dados

Mostrar informações.

JavaScript:

```javascript id="w9r1lc"
console.log("Olá");
```

---

# Boas práticas

✔ Use nomes claros.

✔ Evite variáveis sem necessidade.

✔ Prefira constantes quando possível.

✔ Organize seus dados.

✔ Entenda o tipo de cada informação.

---

# Exercícios

1. O que é uma variável?
2. Qual a diferença entre variável e constante?
3. Cite cinco tipos de dados.
4. Para que serve um boolean?
5. O que significa camelCase?
6. Explique o operador `%`.
7. Qual a diferença entre `=` e `==`?
8. Explique AND e OR.
9. Crie variáveis para armazenar:

   * nome;
   * idade;
   * cidade;
   * altura.
10. Crie um programa que calcule a soma de dois números.

---

# Projeto Prático

Crie um sistema simples de cadastro.

O programa deve armazenar:

```text
Nome

Idade

Email

Cidade

Está ativo?
```

Depois:

* mostre os dados;
* faça comparações;
* utilize operadores.

Exemplo:

```javascript
let nome = "Davi";

let idade = 15;

let ativo = true;

console.log(nome);
console.log(idade);
console.log(ativo);
```

---

# Resumo do capítulo

Neste capítulo você aprendeu:

✅ O que são variáveis.
✅ Como funciona armazenamento de dados.
✅ Diferença entre variável e constante.
✅ Tipos de dados.
✅ Strings, Numbers, Booleans, Arrays e Objects.
✅ Operadores matemáticos.
✅ Operadores de comparação.
✅ Operadores lógicos.
✅ Conversão de tipos.
✅ Entrada e saída de informações.

---

## Próximo capítulo

No **Capítulo 14**, você aprenderá **Estruturas Condicionais**, entendendo como criar programas inteligentes capazes de tomar decisões usando `if`, `else`, `else if`, `switch` e lógica booleana.
