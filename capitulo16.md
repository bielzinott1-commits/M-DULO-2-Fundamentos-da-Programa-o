# CURSO COMPLETO DE PROGRAMAÇÃO

# Do Zero ao Desenvolvedor Full Stack

## Volume 2 – Fundamentos da Programação

# CAPÍTULO 16

# Funções e Organização de Código: Criando Programas Profissionais e Reutilizáveis

> **Objetivo do capítulo:** Ao final deste capítulo, você entenderá o conceito de funções, aprenderá como criar blocos de código reutilizáveis, trabalhar com parâmetros e retornos, organizar projetos maiores e escrever códigos mais profissionais.

---

# Introdução

Nos capítulos anteriores aprendemos:

* variáveis;
* tipos de dados;
* operadores;
* decisões;
* repetições.

Agora imagine criar um sistema grande:

Um aplicativo de banco possui:

* login;
* transferência;
* pagamentos;
* cadastro;
* relatórios.

Se colocarmos tudo em um único arquivo, teremos um problema:

```text id="z8lq42"
milhares de linhas de código
```

Difícil de:

* entender;
* corrigir;
* atualizar.

A solução é dividir o programa em partes menores.

Essas partes são chamadas de:

# Funções

---

# O que é uma função?

Uma função é um bloco de código criado para executar uma tarefa específica.

Pense nela como uma ferramenta.

Exemplo:

Uma calculadora possui funções:

```text id="5d7j3n"
Somar

Subtrair

Multiplicar

Dividir
```

Cada uma faz uma responsabilidade.

---

# Por que usar funções?

Funções permitem:

✅ Reutilizar código.

✅ Evitar repetição.

✅ Organizar programas.

✅ Facilitar manutenção.

✅ Melhorar leitura.

---

# Sem funções

Imagine:

```javascript id="fj72s0"
console.log("Olá Davi");

console.log("Olá João");

console.log("Olá Maria");
```

Temos repetição.

---

# Com função

```javascript id="4mq9tu"
function saudar(nome){

console.log("Olá " + nome);

}

saudar("Davi");

saudar("João");

saudar("Maria");
```

Muito melhor.

---

# Criando uma função

Estrutura básica:

```javascript id="8v9b0m"
function nomeDaFuncao(){

// código

}
```

---

# Exemplo simples

```javascript id="0s8m8k"
function mostrarMensagem(){

console.log("Bem-vindo!");

}
```

Para executar:

```javascript id="8p5z4q"
mostrarMensagem();
```

---

# Chamando uma função

Criar uma função não executa automaticamente.

Exemplo:

```javascript id="4c1qjy"
function teste(){

console.log("Executou");

}
```

Nada acontece.

Precisamos chamar:

```javascript id="i5g0du"
teste();
```

Resultado:

```text id="9v5h1d"
Executou
```

---

# Parâmetros

Parâmetros são valores recebidos pela função.

Exemplo:

```javascript id="9dk4oj"
function saudar(nome){

console.log("Olá " + nome);

}
```

Usando:

```javascript id="w3m6ah"
saudar("Carlos");
```

Resultado:

```text id="l2i7cw"
Olá Carlos
```

---

# Mais de um parâmetro

Exemplo:

```javascript id="p9x7bf"
function somar(a,b){

console.log(a+b);

}

somar(10,5);
```

Resultado:

```text id="q5mx7r"
15
```

---

# Parâmetros x Argumentos

Existe uma diferença:

## Parâmetro

É a variável criada na função.

Exemplo:

```javascript id="s0h8k4"
function somar(a,b)
```

`a` e `b` são parâmetros.

---

## Argumento

É o valor enviado.

Exemplo:

```javascript id="9cgq2r"
somar(10,5)
```

`10` e `5` são argumentos.

---

# Retorno de valores

Muitas funções precisam devolver um resultado.

Usamos:

```text id="o7qv9s"
return
```

---

# Exemplo:

```javascript id="txq5t3"
function somar(a,b){

return a+b;

}

let resultado = somar(5,3);

console.log(resultado);
```

Resultado:

```text id="j3j8o8"
8
```

---

# Por que usar RETURN?

Sem retorno:

```javascript id="2x4i4k"
function somar(a,b){

console.log(a+b);

}
```

A função apenas mostra.

Com retorno:

```javascript id="8zq9v0"
return a+b;
```

O valor pode ser usado depois.

---

# Funções com condições

Exemplo:

Sistema de aprovação:

```javascript id="r6z0bj"
function verificarNota(nota){

if(nota >=7){

return "Aprovado";

}else{

return "Reprovado";

}

}

console.log(verificarNota(8));
```

---

# Funções com loops

Exemplo:

Mostrar números:

```javascript id="4e6t5k"
function contar(){

for(let i=1;i<=5;i++){

console.log(i);

}

}

contar();
```

---

# Funções anônimas

São funções sem nome.

Exemplo:

```javascript id="z4m2v7"
let mensagem = function(){

console.log("Olá");

};
```

---

# Arrow Functions

Forma moderna do JavaScript.

Antes:

```javascript id="a4v0xs"
function somar(a,b){

return a+b;

}
```

Depois:

```javascript id="4u5k1j"
const somar = (a,b)=>{

return a+b;

}
```

Forma curta:

```javascript id="2qj5h3"
const somar = (a,b)=> a+b;
```

---

# Escopo de variáveis

Escopo define onde uma variável pode ser acessada.

---

# Variável local

Existe apenas dentro da função.

Exemplo:

```javascript id="f2w7a3"
function teste(){

let numero = 10;

}
```

Fora da função:

```javascript id="42yd1d"
console.log(numero);
```

Erro.

---

# Variável global

Pode ser acessada em vários lugares.

Exemplo:

```javascript id="8l7h0x"
let nome = "Davi";

function mostrar(){

console.log(nome);

}
```

---

# Boa prática:

Evite muitas variáveis globais.

Elas podem causar problemas.

---

# Organização de código

Um projeto profissional não coloca tudo em um arquivo.

Exemplo ruim:

```text id="m7q2pn"
app.js

5000 linhas
```

---

Exemplo profissional:

```text id="6f8r92"
projeto

src/

├── usuarios.js

├── produtos.js

├── pagamentos.js

└── app.js
```

---

# Separação de responsabilidades

Cada função deve fazer uma coisa.

Ruim:

```javascript id="8y7z3c"
function sistema(){

cadastrarUsuario();

enviarEmail();

gerarRelatorio();

pagarConta();

}
```

---

Melhor:

```javascript id="0c2s9h"
cadastrarUsuario();

enviarEmail();

gerarRelatorio();

pagarConta();
```

---

# Funções puras

Uma função pura:

* recebe dados;
* processa;
* retorna resultado;
* não altera coisas externas.

Exemplo:

```javascript id="gq4m3k"
function dobro(numero){

return numero * 2;

}
```

Entrada:

```text id="a0s3kp"
5
```

Saída:

```text id="e6r9j4"
10
```

---

# Recursão

Uma função chamando ela mesma.

Exemplo:

```javascript id="6t7j4s"
function contar(numero){

if(numero==0){

return;

}

console.log(numero);

contar(numero-1);

}
```

---

# Onde funções são usadas?

Praticamente em tudo.

## Sites

Funções para:

* validar formulário;
* buscar dados;
* alterar telas.

---

## Jogos

Funções para:

* movimentação;
* dano;
* pontuação.

---

## Aplicativos

Funções para:

* login;
* pagamentos;
* notificações.

---

# Boas práticas com funções

## 1. Use nomes claros

Ruim:

```javascript id="t1x5r9"
function x(){}
```

Bom:

```javascript id="w6v0my"
function calcularPreco(){}
```

---

## 2. Funções pequenas

Uma função grande deve ser dividida.

---

## 3. Evite repetir código

Se você escreveu algo várias vezes, talvez precise de uma função.

---

## 4. Faça uma função resolver um problema

Exemplo:

```text id="4ap8pz"
calcularSalario()

validarEmail()

buscarUsuario()
```

---

# Erros comuns

❌ Criar funções enormes.

❌ Nomes sem significado.

❌ Não usar retorno quando necessário.

❌ Colocar tudo no arquivo principal.

❌ Criar funções que fazem várias coisas.

---

# Exercícios

1. O que é uma função?
2. Por que funções são importantes?
3. Qual a diferença entre parâmetro e argumento?
4. Para que serve o return?
5. Explique variável local e global.
6. O que é uma arrow function?
7. Crie uma função que soma dois números.
8. Crie uma função que verifica idade.
9. Crie uma função que percorre um array.
10. Explique por que organizar código é importante.

---

# Projeto Prático

Crie uma calculadora utilizando funções.

Ela deve possuir:

```text id="12mw5a"
somar()

subtrair()

multiplicar()

dividir()
```

Exemplo:

```javascript id="0p8n7z"
function somar(a,b){

return a+b;

}

console.log(somar(10,5));
```

Depois organize:

```text id="a4y6cw"
Calculadora

├── README.md

├── calculadora.js

└── testes.js
```

Publique no GitHub.

---

# Resumo do capítulo

Neste capítulo você aprendeu:

✅ O conceito de funções.
✅ Como criar e chamar funções.
✅ Parâmetros e argumentos.
✅ Retorno de valores.
✅ Arrow Functions.
✅ Escopo de variáveis.
✅ Organização profissional de código.
✅ Separação de responsabilidades.
✅ Funções puras.
✅ Recursão.

---

## Próximo capítulo

No **Capítulo 17**, você aprenderá **Arrays, Listas e Estruturas de Dados**, entendendo como armazenar grandes quantidades de informações, manipular coleções de dados e criar sistemas mais completos.
