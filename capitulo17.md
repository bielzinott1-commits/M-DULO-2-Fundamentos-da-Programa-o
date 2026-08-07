# CURSO COMPLETO DE PROGRAMAÇÃO

# Do Zero ao Desenvolvedor Full Stack

## Volume 2 – Fundamentos da Programação

# CAPÍTULO 17

# Arrays, Listas e Estruturas de Dados: Organizando Grandes Quantidades de Informações

> **Objetivo do capítulo:** Ao final deste capítulo, você entenderá como armazenar vários dados dentro de uma única estrutura, aprenderá a manipular listas, percorrer informações, adicionar e remover elementos e compreenderá uma das bases mais importantes da programação: **estruturas de dados**.

---

# Introdução

Nos capítulos anteriores aprendemos a criar variáveis.

Exemplo:

```javascript id="k1m7as"
let nome = "Davi";

let idade = 15;

let cidade = "Araquari";
```

Isso funciona.

Mas imagine um sistema com:

* 10 mil usuários;
* milhares de produtos;
* milhões de mensagens.

Criar uma variável para cada informação seria impossível.

Exemplo:

```javascript id="p8y4nz"
let usuario1;

let usuario2;

let usuario3;

let usuario4;
```

Precisamos de uma forma melhor.

A solução:

# Arrays e Listas

---

# O que é uma estrutura de dados?

Uma estrutura de dados é uma forma organizada de armazenar informações dentro de um programa.

Ela define:

* como os dados ficam guardados;
* como podem ser acessados;
* como podem ser modificados.

---

# Exemplos de estruturas de dados

Existem várias:

* Arrays;
* Listas;
* Pilhas;
* Filas;
* Árvores;
* Grafos;
* Tabelas.

Cada uma resolve problemas diferentes.

---

# O que é um Array?

Um array é uma coleção de valores armazenados em uma única variável.

Exemplo:

```javascript id="x0m7bg"
let frutas = [
"maçã",
"banana",
"uva"
];
```

Agora temos uma lista:

```text
frutas

[0] maçã

[1] banana

[2] uva
```

---

# Índices dos arrays

Os arrays começam pelo índice:

# 0

Exemplo:

```javascript id="q4h7n3"
let nomes = [
"Ana",
"João",
"Maria"
];
```

Posições:

```text
Índice 0 → Ana

Índice 1 → João

Índice 2 → Maria
```

---

# Acessando valores

Para pegar um item usamos o índice.

Exemplo:

```javascript id="j3r8q1"
console.log(nomes[0]);
```

Resultado:

```text
Ana
```

---

Outro exemplo:

```javascript id="y8s2mz"
console.log(nomes[2]);
```

Resultado:

```text
Maria
```

---

# Alterando valores

Podemos modificar elementos.

Exemplo:

```javascript id="h5p0xv"
let frutas = [
"maçã",
"banana",
"uva"
];

frutas[1] = "laranja";
```

Resultado:

```text
maçã

laranja

uva
```

---

# Tamanho de um array

Usamos:

```javascript id="6r3qwf"
.length
```

Exemplo:

```javascript id="s7z0dq"
let jogos = [
"GTA",
"Minecraft",
"Zelda"
];

console.log(jogos.length);
```

Resultado:

```text
3
```

---

# Adicionando elementos

Existem métodos próprios.

---

# PUSH

Adiciona no final.

Exemplo:

```javascript id="9m3q7t"
let jogos = [
"FIFA",
"Minecraft"
];

jogos.push("GTA");
```

Resultado:

```text
FIFA

Minecraft

GTA
```

---

# UNSHIFT

Adiciona no começo.

Exemplo:

```javascript id="4z8wq2"
jogos.unshift("Zelda");
```

Resultado:

```text
Zelda

FIFA

Minecraft
```

---

# Removendo elementos

---

# POP

Remove o último elemento.

Exemplo:

```javascript id="8v5x1a"
jogos.pop();
```

Antes:

```text
GTA

Minecraft

Zelda
```

Depois:

```text
GTA

Minecraft
```

---

# SHIFT

Remove o primeiro.

Exemplo:

```javascript id="2n6c9h"
jogos.shift();
```

---

# Encontrando elementos

## INDEXOF

Procura posição.

Exemplo:

```javascript id="5q7b2m"
let frutas=[
"maçã",
"banana",
"uva"
];

console.log(frutas.indexOf("banana"));
```

Resultado:

```text
1
```

---

# Verificando existência

Usamos:

```javascript id="d3n6x9"
includes()
```

Exemplo:

```javascript id="1z9c8s"
frutas.includes("uva");
```

Resultado:

```text
true
```

---

# Percorrendo arrays

Uma das tarefas mais comuns.

---

# Usando FOR

Exemplo:

```javascript id="u8m3lp"
let nomes=[
"Ana",
"João",
"Maria"
];

for(let i=0;i<nomes.length;i++){

console.log(nomes[i]);

}
```

Resultado:

```text
Ana

João

Maria
```

---

# Usando FOR OF

Forma mais simples.

Exemplo:

```javascript id="7c5v9q"
for(let nome of nomes){

console.log(nome);

}
```

---

# Usando FOREACH

Outro método moderno:

```javascript id="0h7r3v"
nomes.forEach(function(nome){

console.log(nome);

});
```

---

# Arrays multidimensionais

São arrays dentro de arrays.

Exemplo:

```javascript id="6q9s2a"
let matriz = [

[1,2,3],

[4,5,6],

[7,8,9]

];
```

Representa:

```text
1 2 3

4 5 6

7 8 9
```

Muito usado em:

* jogos;
* mapas;
* tabelas.

---

# Arrays de objetos

Muito usado em sistemas reais.

Exemplo:

```javascript id="k0x6mv"
let usuarios=[

{
nome:"Davi",
idade:15
},

{
nome:"Carlos",
idade:20
}

];
```

---

Acessando:

```javascript id="w1y8z3"
console.log(usuarios[0].nome);
```

Resultado:

```text
Davi
```

---

# Métodos importantes de arrays

JavaScript possui muitos métodos.

---

# MAP

Cria um novo array transformado.

Exemplo:

```javascript id="n9s3wx"
let numeros=[1,2,3];

let dobro = numeros.map(n=>n*2);
```

Resultado:

```text
[2,4,6]
```

---

# FILTER

Filtra informações.

Exemplo:

```javascript id="c6w4hz"
let idades=[10,18,25,15];

let adultos =
idades.filter(idade=>idade>=18);
```

Resultado:

```text
[18,25]
```

---

# REDUCE

Faz cálculos acumulados.

Exemplo:

```javascript id="8b5nq0"
let valores=[10,20,30];

let total =
valores.reduce((a,b)=>a+b);

```

Resultado:

```text
60
```

---

# Ordenando arrays

Método:

```javascript id="s7n4kp"
sort()
```

Exemplo:

```javascript id="3p9x2m"
let numeros=[5,2,8,1];

numeros.sort();
```

Resultado:

```text
1,2,5,8
```

---

# Invertendo valores

Método:

```javascript id="p8r3y0"
reverse()
```

Exemplo:

```javascript
numeros.reverse();
```

---

# Estruturas de dados importantes

Agora vamos conhecer conceitos usados em programação profissional.

---

# Lista

Uma coleção de elementos.

Exemplo:

```text
Lista de usuários
Lista de produtos
Lista de tarefas
```

---

# Pilha (Stack)

Funciona como uma pilha de objetos.

Regra:

# Último que entra, primeiro que sai

Chamado:

```text
LIFO
```

Exemplo:

Pilhas de livros.

---

# Fila (Queue)

Funciona como uma fila.

Regra:

# Primeiro que entra, primeiro que sai

Chamado:

```text
FIFO
```

Exemplo:

Fila de banco.

---

# Árvore (Tree)

Estrutura hierárquica.

Exemplo:

Pastas do computador:

```text
Computador

├── Documentos

├── Fotos

└── Jogos
```

---

# Grafo (Graph)

Conjunto de conexões.

Exemplo:

Redes sociais:

```text
Pessoa

↓

Amigos

↓

Comunidades
```

---

# Onde arrays são usados?

## Redes sociais

Lista de:

* seguidores;
* mensagens;
* publicações.

---

## Jogos

Lista de:

* jogadores;
* itens;
* inimigos.

---

## E-commerce

Lista de:

* produtos;
* pedidos;
* clientes.

---

# Boas práticas

✔ Use nomes no plural.

Exemplo:

Bom:

```javascript
usuarios
```

Ruim:

```javascript
usuario
```

---

✔ Não misture tipos sem necessidade.

Ruim:

```javascript
[10,"Davi",true]
```

---

✔ Organize seus dados.

---

✔ Utilize métodos adequados.

---

# Erros comuns

❌ Esquecer que o índice começa em 0.

❌ Tentar acessar uma posição inexistente.

Exemplo:

```javascript
array[100]
```

❌ Criar arrays gigantes sem organização.

---

# Exercícios

1. O que é um array?
2. Por que arrays são importantes?
3. Por que o índice começa em 0?
4. Explique PUSH e POP.
5. Explique FILTER.
6. O que é uma lista?
7. Explique Stack.
8. Explique Queue.
9. Crie um array de 5 jogos.
10. Percorra esse array usando FOR.

---

# Projeto Prático

Crie um sistema de gerenciamento de jogos.

O sistema deve armazenar:

```text
Nome do jogo

Categoria

Ano

Nota
```

Exemplo:

```javascript
let jogos=[

{
nome:"Minecraft",
categoria:"Sandbox",
ano:2011,
nota:10
}

];
```

O programa deve:

✅ Adicionar jogos.
✅ Remover jogos.
✅ Mostrar todos.
✅ Buscar por nome.
✅ Filtrar por nota.

Depois publique no GitHub.

---

# Resumo do capítulo

Neste capítulo você aprendeu:

✅ O conceito de estruturas de dados.
✅ O que são arrays.
✅ Índices.
✅ Adicionar e remover elementos.
✅ Percorrer listas.
✅ Arrays de objetos.
✅ Métodos MAP, FILTER e REDUCE.
✅ Pilhas e filas.
✅ Árvores e grafos.
✅ Como organizar grandes quantidades de dados.

---

## Próximo capítulo

No **Capítulo 18**, você aprenderá **Programação Orientada a Objetos (POO)**, um dos conceitos mais importantes da programação moderna, usado em jogos, aplicativos, sistemas empresariais e grandes projetos profissionais.
