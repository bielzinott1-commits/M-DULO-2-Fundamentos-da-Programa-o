# CURSO COMPLETO DE PROGRAMAÇÃO

# Do Zero ao Desenvolvedor Full Stack

## Volume 2 – Fundamentos da Programação

# CAPÍTULO 18

# Programação Orientada a Objetos (POO): Criando Sistemas Organizados e Profissionais

> **Objetivo do capítulo:** Ao final deste capítulo, você entenderá o conceito de Programação Orientada a Objetos, aprenderá a criar classes, objetos, atributos, métodos, compreenderá encapsulamento, herança e polimorfismo, além de entender por que a POO é tão utilizada no desenvolvimento profissional.

---

# Introdução

Até agora aprendemos programação utilizando:

* variáveis;
* funções;
* condições;
* loops;
* arrays.

Esse estilo é chamado de:

# Programação Estruturada

Ela funciona muito bem para programas pequenos.

Porém, imagine criar:

* um jogo completo;
* uma rede social;
* um sistema bancário;
* um aplicativo de comércio.

Esses sistemas possuem milhares de informações relacionadas.

Exemplo:

Um jogo possui:

```text
Personagem

- Nome
- Vida
- Energia
- Inventário

Ações:

- Andar
- Atacar
- Defender
```

Organizar tudo apenas com variáveis e funções fica complicado.

A solução é:

# Programação Orientada a Objetos (POO)

---

# O que é Programação Orientada a Objetos?

POO é um paradigma de programação baseado na criação de objetos que representam coisas do mundo real.

A ideia principal:

> Transformar elementos reais em estruturas dentro do programa.

---

# Exemplos de objetos reais

Um carro possui:

Características:

```text
Marca

Modelo

Cor

Ano
```

Ações:

```text
Ligar

Acelerar

Frear
```

Na programação:

```text
Objeto Carro

Atributos:

marca
modelo
cor

Métodos:

ligar()
acelerar()
frear()
```

---

# O que é um objeto?

Um objeto é uma entidade que possui:

## Dados

Chamados de:

# Atributos

Exemplo:

```text
Nome
Idade
Email
```

---

## Comportamentos

Chamados de:

# Métodos

Exemplo:

```text
Enviar mensagem

Comprar produto

Fazer login
```

---

# O que é uma classe?

Uma classe é um modelo usado para criar objetos.

Pense em uma planta de uma casa.

A planta não é a casa.

Ela apenas define como a casa será.

Na programação:

```text
Classe = Modelo

Objeto = Instância criada
```

---

# Exemplo:

Classe:

```text
Pessoa
```

Objetos:

```text
Davi

Carlos

Maria
```

Todos são pessoas, mas possuem informações diferentes.

---

# Criando uma classe

Exemplo em JavaScript:

```javascript id="n8q4xu"
class Pessoa {

}
```

Criamos uma classe chamada:

```text
Pessoa
```

---

# Criando atributos

Usamos o:

```text
constructor
```

Ele é executado quando criamos um objeto.

Exemplo:

```javascript id="4q2j9h"
class Pessoa{

constructor(nome,idade){

this.nome = nome;

this.idade = idade;

}

}
```

---

# Criando objetos

Agora podemos criar pessoas:

```javascript id="6v7m8k"
let pessoa1 = new Pessoa("Davi",15);

let pessoa2 = new Pessoa("Carlos",20);
```

Temos:

```text
Pessoa 1

Nome: Davi
Idade: 15


Pessoa 2

Nome: Carlos
Idade: 20
```

---

# O que é o THIS?

`this` representa o próprio objeto.

Exemplo:

```javascript id="x5q9sa"
this.nome = nome;
```

Significa:

"O nome deste objeto recebe o valor informado."

---

# Métodos

Métodos são funções dentro de uma classe.

Exemplo:

```javascript id="3p4h8d"
class Pessoa{

constructor(nome){

this.nome = nome;

}


apresentar(){

console.log("Olá " + this.nome);

}

}
```

Usando:

```javascript id="8t5h9j"
let pessoa = new Pessoa("Davi");

pessoa.apresentar();
```

Resultado:

```text
Olá Davi
```

---

# A diferença entre função e método

Função:

```javascript
function calcular(){

}
```

Existe sozinha.

---

Método:

```javascript
objeto.calcular()
```

Pertence a um objeto.

---

# Os quatro pilares da POO

A Programação Orientada a Objetos possui quatro conceitos principais:

1. Encapsulamento
2. Herança
3. Polimorfismo
4. Abstração

---

# 1. Encapsulamento

Encapsulamento significa proteger informações internas de um objeto.

Exemplo:

Um banco não permite alterar seu saldo diretamente.

Errado:

```text
saldo = 1000000
```

O correto:

```text
depositar()

sacar()
```

---

Na programação:

```javascript id="7v5w8m"
class Conta{

constructor(){

this.saldo = 0;

}


depositar(valor){

this.saldo += valor;

}

}
```

O controle fica dentro do objeto.

---

# Benefícios do encapsulamento:

✅ Segurança.

✅ Organização.

✅ Controle dos dados.

---

# 2. Herança

Herança permite que uma classe receba características de outra.

Exemplo:

Classe:

```text
Animal
```

Possui:

```text
Nome

Idade

Comer()
```

---

Outras classes:

```text
Cachorro

Gato
```

Podem herdar:

```text
Nome

Idade

Comer()
```

---

Exemplo JavaScript:

```javascript id="7w3y8p"
class Animal{

comer(){

console.log("Comendo");

}

}


class Cachorro extends Animal{


latir(){

console.log("Au au");

}


}
```

Agora:

```javascript id="j4h9r2"
let cachorro = new Cachorro();

cachorro.comer();
```

Funciona.

---

# 3. Polimorfismo

Polimorfismo significa:

"Várias formas"

Objetos diferentes podem responder ao mesmo comando de maneiras diferentes.

Exemplo:

Animal:

```text
fazerSom()
```

Cachorro:

```text
Au au
```

Gato:

```text
Miau
```

---

Código:

```javascript id="p8v6w0"
class Animal{

fazerSom(){

}

}


class Cachorro extends Animal{

fazerSom(){

console.log("Au au");

}

}


class Gato extends Animal{

fazerSom(){

console.log("Miau");

}

}
```

---

# 4. Abstração

Abstração significa esconder detalhes desnecessários.

Exemplo:

Você dirige um carro.

Você usa:

* volante;
* pedal;
* câmbio.

Mas não precisa saber:

* funcionamento do motor;
* combustão;
* eletrônica.

---

Na programação:

O usuário usa uma função simples.

Por trás existe muita complexidade.

---

# Classes abstratas

São modelos que não devem ser usados diretamente.

Exemplo:

```text
Animal

não é um animal específico.

É apenas uma categoria.
```

---

# POO em diferentes linguagens

A POO existe em várias linguagens:

## Java

Muito utilizada em empresas.

---

## C++

Usada em:

* jogos;
* sistemas de alto desempenho.

---

## C#

Usada em:

* Unity;
* aplicações Microsoft.

---

## Python

Possui suporte completo a POO.

---

## JavaScript

Possui classes modernas.

---

# Exemplos reais de POO

## Jogos

Classe:

```text
Personagem
```

Objetos:

```text
Guerreiro

Mago

Arqueiro
```

---

## Aplicativo bancário

Classes:

```text
Cliente

Conta

Transação
```

---

## Loja virtual

Classes:

```text
Produto

Carrinho

Pedido

Cliente
```

---

# Organização profissional com POO

Um projeto pode ser dividido:

```text
Sistema

src/

├── Usuario.js

├── Produto.js

├── Pedido.js

└── Banco.js
```

Cada classe possui sua responsabilidade.

---

# Boas práticas

## 1. Classes com nomes claros

Bom:

```text
Usuario

Produto

Pagamento
```

Ruim:

```text
Classe1
```

---

## 2. Uma classe deve ter uma responsabilidade

Evite:

```text
Classe SistemaFazTudo
```

---

## 3. Não abuse da herança

Às vezes composição é melhor.

---

# Erros comuns de iniciantes

❌ Criar classes sem necessidade.

❌ Misturar muitas responsabilidades.

❌ Não entender objetos antes de criar classes.

❌ Usar POO apenas porque é "mais profissional".

---

# Exercícios

1. O que é POO?
2. Qual a diferença entre classe e objeto?
3. O que são atributos?
4. O que são métodos?
5. Explique encapsulamento.
6. Explique herança.
7. Explique polimorfismo.
8. Explique abstração.
9. Crie uma classe Carro.
10. Crie uma classe Usuario com métodos.

---

# Projeto Prático

Crie um sistema de personagens de jogo.

Classe:

```text
Personagem
```

Atributos:

```text
Nome

Vida

Ataque

Defesa
```

Métodos:

```text
Atacar()

Defender()

MostrarStatus()
```

Depois crie:

```text
Guerreiro

Mago

Arqueiro
```

Utilizando herança.

Publique no GitHub com:

* README;
* código organizado;
* exemplos de uso.

---

# Resumo do capítulo

Neste capítulo você aprendeu:

✅ O conceito de Programação Orientada a Objetos.
✅ Classes e objetos.
✅ Atributos e métodos.
✅ Constructor.
✅ THIS.
✅ Encapsulamento.
✅ Herança.
✅ Polimorfismo.
✅ Abstração.
✅ Uso da POO em projetos reais.

---

## Próximo capítulo

No **Capítulo 19**, você aprenderá **Banco de Dados e Armazenamento de Informações**, entendendo como sistemas profissionais salvam usuários, produtos, mensagens e grandes volumes de dados usando bancos SQL e NoSQL.
