# CURSO COMPLETO DE PROGRAMAÇÃO

# Do Zero ao Desenvolvedor Full Stack

## Volume 2 – Fundamentos da Programação

# CAPÍTULO 15

# Estruturas de Repetição (Loops): Ensinando o Computador a Repetir Tarefas

> **Objetivo do capítulo:** Ao final deste capítulo, você entenderá como criar programas capazes de repetir ações automaticamente, aprenderá os principais tipos de loops (`for`, `while`, `do while`) e saberá quando utilizar cada estrutura em projetos reais.

---

# Introdução

Imagine que você precise criar um programa que mostre:

```text
Olá
Olá
Olá
Olá
Olá
```

Você poderia escrever:

```javascript
console.log("Olá");
console.log("Olá");
console.log("Olá");
console.log("Olá");
console.log("Olá");
```

Funciona.

Mas imagine fazer isso:

```text
Mostrar "Olá" 1 milhão de vezes.
```

Seria impossível escrever manualmente.

Para resolver esse problema existem:

# Estruturas de Repetição

Também chamadas de:

* Loops;
* Laços de repetição.

---

# O que é um loop?

Um loop é uma estrutura que permite executar um bloco de código várias vezes.

Exemplo:

```text
Enquanto uma condição for verdadeira:

    execute uma ação
```

---

# Exemplos do mundo real

## Relógio

Um relógio repete:

```text
Atualizar hora

Esperar 1 segundo

Atualizar hora novamente
```

---

## Jogo

Um jogo executa constantemente:

```text
Verificar movimento

Atualizar posição

Renderizar tela
```

---

## Rede social

Um aplicativo mostra:

```text
Para cada postagem:

Mostrar publicação
```

---

# Por que usar loops?

Loops ajudam a:

✅ Evitar código repetido.

✅ Automatizar tarefas.

✅ Trabalhar com grandes quantidades de dados.

✅ Criar sistemas eficientes.

---

# Tipos principais de loops

As principais estruturas são:

1. `for`
2. `while`
3. `do while`

---

# 1. Loop FOR

O `for` é utilizado quando sabemos quantas vezes queremos repetir algo.

Estrutura:

```javascript
for(início; condição; incremento){

    código

}
```

Ele possui três partes:

---

## 1. Inicialização

Onde começa.

Exemplo:

```javascript
let contador = 0;
```

---

## 2. Condição

Até quando continua.

Exemplo:

```javascript
contador < 10;
```

---

## 3. Incremento

Como aumenta.

Exemplo:

```javascript
contador++;
```

---

# Exemplo básico

```javascript
for(let contador = 1; contador <= 5; contador++){

console.log(contador);

}
```

Resultado:

```text
1
2
3
4
5
```

---

# Entendendo passo a passo

Primeira execução:

```text
contador = 1
```

Verifica:

```text
1 <= 5?
```

Sim.

Mostra:

```text
1
```

Depois:

```text
contador++
```

Agora:

```text
2
```

Repete até chegar em 5.

---

# Contador crescente

Exemplo:

```javascript
for(let i = 0; i < 10; i++){

console.log(i);

}
```

Resultado:

```text
0
1
2
3
4
5
6
7
8
9
```

---

# Contador decrescente

Também podemos diminuir.

Exemplo:

```javascript
for(let i = 10; i >= 0; i--){

console.log(i);

}
```

Resultado:

```text
10
9
8
7
...
0
```

---

# Operadores de incremento

## Somar 1

```javascript
i++;
```

É igual:

```javascript
i = i + 1;
```

---

## Diminuir 1

```javascript
i--;
```

É igual:

```javascript
i = i - 1;
```

---

# Usando FOR com arrays

Arrays possuem vários valores.

Exemplo:

```javascript
let frutas = [
"maçã",
"banana",
"uva"
];
```

Podemos percorrer:

```javascript
for(let i = 0; i < frutas.length; i++){

console.log(frutas[i]);

}
```

Resultado:

```text
maçã

banana

uva
```

---

# O que é LENGTH?

`length` mostra o tamanho de uma lista.

Exemplo:

```javascript
let nomes = ["Ana","João","Maria"];

console.log(nomes.length);
```

Resultado:

```text
3
```

---

# 2. Loop WHILE

O `while` significa:

"enquanto"

Ele continua enquanto uma condição for verdadeira.

Estrutura:

```javascript
while(condição){

código

}
```

---

# Exemplo:

```javascript
let contador = 1;

while(contador <= 5){

console.log(contador);

contador++;

}
```

Resultado:

```text
1
2
3
4
5
```

---

# Diferença entre FOR e WHILE

## FOR

Use quando sabe a quantidade de repetições.

Exemplo:

```text
Mostrar 10 números.
```

---

## WHILE

Use quando depende de uma condição.

Exemplo:

```text
Enquanto o usuário não sair:

continuar executando
```

---

# Exemplo real com WHILE

Sistema de senha:

```javascript
let senha = "";

while(senha != "1234"){

senha = "1234";

}

console.log("Acesso liberado");
```

---

# 3. Loop DO WHILE

O `do while` é parecido com o while.

A diferença:

Ele executa pelo menos uma vez.

Estrutura:

```javascript
do{

código

}while(condição);
```

---

# Exemplo:

```javascript
let numero = 1;

do{

console.log(numero);

numero++;

}while(numero <= 5);
```

Resultado:

```text
1
2
3
4
5
```

---

# Diferença entre WHILE e DO WHILE

## WHILE

Primeiro verifica.

Depois executa.

Exemplo:

```text
Condição?

Sim → executa
Não → pula
```

---

## DO WHILE

Primeiro executa.

Depois verifica.

Exemplo:

```text
Executa

↓

Condição?
```

---

# Controle de loops

Existem comandos especiais:

* break;
* continue.

---

# BREAK

O `break` interrompe o loop.

Exemplo:

```javascript
for(let i = 1; i <=10; i++){

if(i == 5){

break;

}

console.log(i);

}
```

Resultado:

```text
1
2
3
4
```

Quando chega no 5, para.

---

# CONTINUE

O `continue` pula uma repetição.

Exemplo:

```javascript
for(let i = 1; i <=5; i++){

if(i == 3){

continue;

}

console.log(i);

}
```

Resultado:

```text
1
2
4
5
```

O número 3 foi ignorado.

---

# Loops aninhados

Um loop dentro de outro.

Exemplo:

Criar uma tabela:

```javascript
for(let linha = 1; linha <=3; linha++){

for(let coluna = 1; coluna <=3; coluna++){

console.log(linha,coluna);

}

}
```

Resultado:

```text
1 1
1 2
1 3
2 1
2 2
2 3
3 1
3 2
3 3
```

---

# Loops em sistemas reais

## Loja virtual

Percorrer produtos:

```javascript
for(cada produto){

mostrar produto

}
```

---

## Banco

Verificar transações:

```javascript
for(cada movimentação){

calcular saldo

}
```

---

## Jogos

Atualização:

```javascript
while(jogoAtivo){

atualizar jogo

}
```

---

# Erros comuns com loops

## 1. Loop infinito

Exemplo:

```javascript
while(true){

console.log("Olá");

}
```

Nunca termina.

---

## 2. Esquecer incremento

Errado:

```javascript
let i = 0;

while(i < 10){

console.log(i);

}
```

O valor nunca muda.

---

Correto:

```javascript
i++;
```

---

## 3. Condição errada

Exemplo:

```javascript
for(let i=10;i<5;i++)
```

Nunca executará.

---

# Boas práticas

✔ Sempre saiba quando o loop termina.

✔ Use nomes claros.

✔ Evite loops gigantes.

✔ Teste com poucos dados primeiro.

✔ Utilize métodos modernos quando necessário.

---

# Exercícios

1. O que é um loop?
2. Por que usamos estruturas de repetição?
3. Qual a diferença entre FOR e WHILE?
4. Explique o DO WHILE.
5. Para que serve o BREAK?
6. Para que serve o CONTINUE?
7. Crie um loop que mostre números de 1 até 100.
8. Crie um loop que conte de 10 até 0.
9. Percorra um array de nomes usando FOR.
10. Explique o que é um loop infinito.

---

# Projeto Prático

Crie um sistema de cadastro de produtos.

O programa deve:

Armazenar:

```text
Produto 1
Produto 2
Produto 3
Produto 4
Produto 5
```

Depois:

* percorrer todos os produtos;
* mostrar na tela;
* contar quantos existem.

Exemplo:

```javascript
let produtos = [
"Teclado",
"Mouse",
"Monitor"
];

for(let i = 0; i < produtos.length; i++){

console.log(produtos[i]);

}
```

---

# Resumo do capítulo

Neste capítulo você aprendeu:

✅ O que são loops.
✅ Por que repetição é importante.
✅ Estrutura FOR.
✅ Estrutura WHILE.
✅ Estrutura DO WHILE.
✅ Incrementos e decrementos.
✅ Percorrer arrays.
✅ BREAK e CONTINUE.
✅ Loops aninhados.
✅ Como evitar loops infinitos.

---

## Próximo capítulo

No **Capítulo 16**, você aprenderá **Funções e Organização de Código**, entendendo como criar blocos reutilizáveis, diminuir repetição, organizar programas grandes e começar a programar de forma mais profissional.
