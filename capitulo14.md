# CURSO COMPLETO DE PROGRAMAÇÃO

# Do Zero ao Desenvolvedor Full Stack

## Volume 2 – Fundamentos da Programação

# CAPÍTULO 14

# Estruturas Condicionais: Ensinando o Programa a Tomar Decisões

> **Objetivo do capítulo:** Ao final deste capítulo, você entenderá como criar programas capazes de analisar situações, tomar decisões automaticamente e executar diferentes ações utilizando condições como `if`, `else`, `else if` e `switch`.

---

# Introdução

Até agora aprendemos que um programa pode:

* armazenar informações;
* realizar cálculos;
* mostrar resultados.

Mas existe um problema:

E se o programa precisar **escolher um caminho diferente dependendo da situação?**

Exemplo:

Um aplicativo de banco precisa decidir:

```
Se a senha estiver correta:
    liberar acesso

Senão:
    bloquear acesso
```

Um jogo precisa decidir:

```
Se a vida for menor que zero:
    personagem morreu
```

Essa capacidade de decisão é criada usando:

# Estruturas Condicionais

---

# O que é uma condição?

Uma condição é uma pergunta que pode ter apenas dois resultados:

```
Verdadeiro (true)

ou

Falso (false)
```

Exemplo:

Pergunta:

```
A idade é maior ou igual a 18?
```

Possíveis respostas:

```
Sim → true

Não → false
```

---

# Como computadores tomam decisões?

O computador segue regras.

Exemplo:

```text
SE uma condição for verdadeira

execute uma ação

SENÃO

execute outra ação
```

Essa estrutura aparece em praticamente todos os sistemas.

---

# Exemplos de decisões na vida real

## Exemplo 1: Chuva

```
SE estiver chovendo

pegar guarda-chuva

SENÃO

sair normalmente
```

---

## Exemplo 2: Login

```
SE usuário e senha estiverem corretos

entrar no sistema

SENÃO

mostrar erro
```

---

## Exemplo 3: Jogo

```
SE vida <= 0

personagem morreu
```

---

# Operadores de comparação

As condições utilizam comparações.

| Operador | Significado    |
| -------- | -------------- |
| ==       | Igual          |
| !=       | Diferente      |
| >        | Maior          |
| <        | Menor          |
| >=       | Maior ou igual |
| <=       | Menor ou igual |

---

# Estrutura IF

`if` significa:

"se"

Ele executa um código quando uma condição é verdadeira.

Estrutura:

```javascript
if(condição){

    código

}
```

---

# Exemplo simples

```javascript
let idade = 18;

if(idade >= 18){

console.log("Pode entrar");

}
```

Resultado:

```
Pode entrar
```

---

# Entendendo o código

Temos:

```javascript
idade >= 18
```

O computador pergunta:

```
18 é maior ou igual a 18?
```

Resposta:

```
true
```

Então executa:

```javascript
console.log("Pode entrar");
```

---

# Estrutura IF e ELSE

Agora podemos criar uma alternativa.

Estrutura:

```javascript
if(condição){

    ação 1

}else{

    ação 2

}
```

---

# Exemplo:

```javascript
let idade = 15;

if(idade >= 18){

console.log("Maior de idade");

}else{

console.log("Menor de idade");

}
```

Resultado:

```
Menor de idade
```

---

# Como funciona?

O programa verifica:

```
idade >= 18?
```

Resultado:

```
false
```

Então executa:

```
else
```

---

# Estrutura ELSE IF

Às vezes precisamos de várias possibilidades.

Exemplo:

Sistema de notas:

```
9 ou 10 → Excelente

7 ou 8 → Aprovado

Menor que 7 → Reprovado
```

Código:

```javascript
let nota = 8;

if(nota >= 9){

console.log("Excelente");

}else if(nota >= 7){

console.log("Aprovado");

}else{

console.log("Reprovado");

}
```

---

# Ordem das condições

A ordem importa.

Exemplo errado:

```javascript
let nota = 10;

if(nota >= 5){

console.log("Aprovado");

}else if(nota >= 9){

console.log("Excelente");

}
```

O programa nunca chega no excelente.

Porque 10 também é maior que 5.

---

Forma correta:

```javascript
if(nota >= 9){

console.log("Excelente");

}else if(nota >= 5){

console.log("Aprovado");

}
```

---

# Condições usando AND

O operador:

```
&&
```

significa:

"E"

As duas condições precisam ser verdadeiras.

Exemplo:

Sistema de entrada:

```javascript
let idade = 20;
let ingresso = true;

if(idade >=18 && ingresso == true){

console.log("Entrada permitida");

}
```

Para entrar:

* precisa ter idade;
* precisa ter ingresso.

---

# Condições usando OR

O operador:

```
||
```

significa:

"OU"

Apenas uma condição precisa ser verdadeira.

Exemplo:

```javascript
let pagamento = "pix";

if(pagamento=="pix" || pagamento=="cartao"){

console.log("Pagamento aceito");

}
```

---

# Negação com NOT

Operador:

```
!
```

Inverte um valor.

Exemplo:

```javascript
let bloqueado = false;

if(!bloqueado){

console.log("Usuário liberado");

}
```

---

# Condições dentro de condições

Chamamos de:

# Condicionais aninhadas

Exemplo:

```javascript
let usuario = true;
let senha = true;

if(usuario){

    if(senha){

        console.log("Login realizado");

    }

}
```

---

# Switch Case

Quando temos muitas opções, usamos:

```
switch
```

Exemplo:

Menu de aplicativo:

```
1 - Início

2 - Perfil

3 - Configurações
```

Código:

```javascript
let opcao = 2;

switch(opcao){

case 1:

console.log("Início");

break;


case 2:

console.log("Perfil");

break;


case 3:

console.log("Configurações");

break;


default:

console.log("Opção inválida");

}
```

---

# O que é BREAK?

O comando:

```
break
```

encerra o bloco.

Sem ele, o programa continua executando os próximos casos.

---

# O que é DEFAULT?

É executado quando nenhuma opção combina.

Exemplo:

Usuário digita:

```
5
```

Resultado:

```
Opção inválida
```

---

# Comparação de IF e SWITCH

## IF

Melhor para:

* intervalos;
* cálculos;
* condições complexas.

Exemplo:

```javascript
idade >= 18
```

---

## SWITCH

Melhor para:

* menus;
* opções fixas;
* escolhas.

Exemplo:

```text
1
2
3
```

---

# Exemplos reais de condicionais

## Sistema bancário

```javascript
if(saldo >= valor){

console.log("Transferência realizada");

}else{

console.log("Saldo insuficiente");

}
```

---

## Loja virtual

```javascript
if(compra >= 200){

console.log("Frete grátis");

}else{

console.log("Frete pago");

}
```

---

## Jogo

```javascript
if(vida <= 0){

console.log("Game Over");

}
```

---

# Operador ternário

Uma forma curta de escrever IF/ELSE.

Estrutura:

```javascript
condição ? verdadeiro : falso
```

Exemplo:

```javascript
let idade = 20;

let resultado = idade >=18 ? "Adulto" : "Menor";

console.log(resultado);
```

Resultado:

```
Adulto
```

---

# Boas práticas

## 1. Use nomes claros

Ruim:

```javascript
if(x){
}
```

Bom:

```javascript
if(usuarioAtivo){
}
```

---

## 2. Evite condições gigantes

Ruim:

```javascript
if(a && b && c && d && e){
}
```

Divida em partes.

---

## 3. Sempre pense nos casos de erro

Exemplo:

Login:

* senha correta;
* senha errada;
* usuário inexistente.

---

# Erros comuns

❌ Confundir `=` com `==`.

Errado:

```javascript
if(idade = 18)
```

Correto:

```javascript
if(idade == 18)
```

---

❌ Esquecer chaves.

Errado:

```javascript
if(valor > 10)

console.log(valor);
```

Melhor:

```javascript
if(valor > 10){

console.log(valor);

}
```

---

❌ Criar condições impossíveis.

Exemplo:

```javascript
if(idade > 18 && idade < 5)
```

Nunca será verdadeiro.

---

# Exercícios

1. O que é uma condição?
2. Qual a diferença entre IF e ELSE?
3. Para que serve ELSE IF?
4. Explique o operador AND.
5. Explique o operador OR.
6. Quando usar SWITCH?
7. Crie um programa que verifica se uma pessoa pode votar.
8. Crie um sistema que verifica aprovação escolar.
9. Crie um menu usando SWITCH.
10. Explique o operador ternário.

---

# Projeto Prático

Crie um sistema de avaliação de aluno.

O programa deve receber:

```
Nome

Nota
```

Regras:

```
Nota >= 9
Excelente

Nota >= 7
Aprovado

Nota >= 5
Recuperação

Nota < 5
Reprovado
```

Depois crie:

✅ Algoritmo
✅ Fluxograma
✅ Pseudocódigo
✅ Código em JavaScript

---

# Resumo do capítulo

Neste capítulo você aprendeu:

✅ O que são estruturas condicionais.
✅ Como computadores tomam decisões.
✅ Uso do IF.
✅ Uso do ELSE.
✅ Uso do ELSE IF.
✅ Uso do SWITCH CASE.
✅ Operadores lógicos.
✅ Operador ternário.
✅ Como criar sistemas inteligentes.

---

## Próximo capítulo

No **Capítulo 15**, você aprenderá **Estruturas de Repetição (Loops)**: como ensinar o computador a repetir tarefas automaticamente usando `for`, `while` e `do while`, uma das habilidades mais importantes da programação.
