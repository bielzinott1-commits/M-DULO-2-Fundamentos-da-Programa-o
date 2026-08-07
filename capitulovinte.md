# CURSO COMPLETO DE PROGRAMAÇÃO

# Do Zero ao Desenvolvedor Full Stack

## Volume 3 – Desenvolvimento Web

# CAPÍTULO 20

# Desenvolvimento Web: HTML, CSS e JavaScript — Criando Sites e Aplicações Modernas

> **Objetivo do capítulo:** Ao final deste capítulo, você entenderá como a internet funciona, como sites são construídos, qual a função do HTML, CSS e JavaScript, como criar páginas web e como essas tecnologias formam a base do desenvolvimento Front-End.

---

# Introdução

Hoje praticamente tudo está conectado à internet.

Quando você acessa:

* Google;
* YouTube;
* Instagram;
* lojas virtuais;
* sistemas empresariais;

existe um conjunto de tecnologias trabalhando por trás.

Um site moderno é construído principalmente com três tecnologias:

# HTML

Estrutura.

# CSS

Visual e design.

# JavaScript

Interatividade e lógica.

---

# Como funciona a internet?

Quando você acessa um site:

Exemplo:

```text id="y6s4kv"
www.exemplo.com
```

Acontece uma comunicação:

```
Usuário

↓

Navegador

↓

Internet

↓

Servidor

↓

Banco de Dados

↓

Resposta para o usuário
```

---

# O que é um navegador?

O navegador é o programa responsável por interpretar códigos da web.

Exemplos:

* Google Chrome;
* Microsoft Edge;
* Firefox;
* Safari.

Ele transforma código em uma página visual.

---

# O que é Front-End?

Front-End é a parte do sistema que o usuário vê e utiliza.

Exemplos:

* botões;
* menus;
* imagens;
* animações;
* telas.

Tecnologias principais:

* HTML;
* CSS;
* JavaScript.

---

# O que é Back-End?

Back-End é a parte que fica por trás.

Responsável por:

* servidores;
* banco de dados;
* autenticação;
* regras do sistema.

Exemplos:

* Node.js;
* Java;
* Python;
* C#.

---

# O que é Full Stack?

Um desenvolvedor Full Stack domina:

## Front-End

Interface.

*

## Back-End

Servidor e dados.

*

## Banco de Dados

Armazenamento.

---

# Estrutura de uma aplicação web

Um sistema completo:

```
Usuário

↓

HTML/CSS/JavaScript

↓

Servidor

↓

Banco de Dados
```

---

# PARTE 1 — HTML

# O que é HTML?

HTML significa:

# HyperText Markup Language

É a linguagem responsável pela estrutura de uma página.

Ele define:

* títulos;
* textos;
* imagens;
* links;
* formulários.

---

# HTML não é linguagem de programação

HTML é uma:

# Linguagem de marcação

Ele organiza informações.

---

# Primeiro arquivo HTML

Criamos:

```
index.html
```

Código:

```html id="8q9z5x"
<!DOCTYPE html>

<html>

<head>

<title>Meu Site</title>

</head>


<body>

<h1>Olá Mundo</h1>

</body>


</html>
```

---

# Estrutura básica HTML

## DOCTYPE

Informa o tipo do documento.

```html
<!DOCTYPE html>
```

---

## HTML

Elemento principal.

```html
<html>
</html>
```

---

## HEAD

Informações da página.

Inclui:

* título;
* configurações;
* links.

---

## BODY

Conteúdo visível.

Exemplo:

* textos;
* imagens;
* botões.

---

# Tags HTML

HTML utiliza:

# Tags

Exemplo:

```html
<h1>Título</h1>
```

Abertura:

```html
<h1>
```

Fechamento:

```html
</h1>
```

---

# Principais tags

## Títulos

```html
<h1>Título principal</h1>

<h2>Subtítulo</h2>

<h3>Outro título</h3>
```

---

## Parágrafo

```html
<p>
Meu texto.
</p>
```

---

## Link

```html
<a href="https://site.com">
Acessar
</a>
```

---

## Imagem

```html
<img src="imagem.png">
```

---

## Lista

Lista ordenada:

```html
<ol>

<li>Item 1</li>

<li>Item 2</li>

</ol>
```

---

Lista sem ordem:

```html
<ul>

<li>Item</li>

</ul>
```

---

# Formulários HTML

Usados para receber informações.

Exemplo:

```html
<form>

<input type="text">

<input type="password">

<button>
Enviar
</button>

</form>
```

---

# PARTE 2 — CSS

# O que é CSS?

CSS significa:

# Cascading Style Sheets

É responsável pelo visual.

Ele controla:

* cores;
* tamanhos;
* posições;
* animações;
* responsividade.

---

# HTML sem CSS

Seria apenas:

```
Texto
Imagem
Botão
```

CSS transforma em:

```
Design profissional
Interface bonita
Experiência agradável
```

---

# Como adicionar CSS

Criamos:

```
style.css
```

Exemplo:

```css
body{

background:white;

font-family:Arial;

}
```

---

# Seletores CSS

Selecionam elementos.

---

## Por tag

```css
h1{

color:red;

}
```

---

## Por classe

HTML:

```html
<p class="texto">
Olá
</p>
```

CSS:

```css
.texto{

font-size:20px;

}
```

---

## Por ID

HTML:

```html
<div id="menu">

</div>
```

CSS:

```css
#menu{

background:black;

}
```

---

# Propriedades importantes

## Cor

```css
color:blue;
```

---

## Fundo

```css
background:red;
```

---

## Tamanho

```css
width:300px;
height:200px;
```

---

## Espaçamento

Margem:

```css
margin:20px;
```

Espaço interno:

```css
padding:20px;
```

---

# Flexbox

Uma das ferramentas mais importantes do CSS.

Serve para organizar elementos.

Exemplo:

```css
.container{

display:flex;

justify-content:center;

align-items:center;

}
```

Usado em:

* menus;
* cards;
* layouts.

---

# Responsividade

Um site precisa funcionar em:

* computador;
* celular;
* tablet.

Usamos:

# Media Queries

Exemplo:

```css
@media(max-width:600px){

body{

font-size:14px;

}

}
```

---

# PARTE 3 — JavaScript

# O que é JavaScript?

JavaScript é a linguagem que adiciona comportamento aos sites.

Com ele podemos criar:

* animações;
* sistemas;
* validações;
* jogos;
* aplicações completas.

---

# Primeiro código JavaScript

```javascript
console.log("Olá mundo");
```

---

# Alterando HTML

HTML:

```html
<p id="texto">
Olá
</p>
```

JavaScript:

```javascript
document.getElementById("texto").innerHTML="Novo texto";
```

---

# Eventos

Eventos são ações do usuário.

Exemplos:

* clicar;
* passar mouse;
* digitar.

---

Exemplo:

```html
<button onclick="mostrar()">

Clique

</button>
```

JavaScript:

```javascript
function mostrar(){

alert("Olá");

}
```

---

# Manipulação do DOM

DOM significa:

# Document Object Model

É a forma que JavaScript acessa elementos HTML.

Exemplo:

```javascript
document.querySelector("h1");
```

---

# Criando interatividade

Exemplo:

Contador:

```javascript
let numero = 0;


function aumentar(){

numero++;

console.log(numero);

}
```

---

# Ferramentas de desenvolvimento web

Programadores utilizam:

## Editor

Microsoft

Muito usado para escrever código.

---

## Navegador

Ferramentas de desenvolvedor:

* Console;
* Inspecionar elemento;
* Debug.

---

## Controle de versão

GitHub

Usado para:

* guardar projetos;
* colaborar;
* mostrar portfólio.

---

# Estrutura profissional de projeto web

Exemplo:

```
meu-site/

├── index.html

├── css/

│   └── style.css

├── js/

│   └── script.js

└── imagens/
```

---

# Projeto completo simples

## HTML

```html
<h1>
Minha página
</h1>

<button onclick="mensagem()">
Clique
</button>
```

---

## JavaScript

```javascript
function mensagem(){

alert("Bem-vindo!");

}
```

---

## CSS

```css
h1{

color:blue;

}
```

Resultado:

Um site simples com:

* título;
* botão;
* interação.

---

# Frameworks modernos

Depois de dominar HTML, CSS e JavaScript, existem ferramentas avançadas.

## Front-End:

* React;
* Angular;
* Vue.

---

## Mobile:

* React Native;
* Flutter.

---

## Back-End JavaScript:

* Node.js.

---

# Boas práticas

✔ Organize arquivos.

✔ Use nomes claros.

✔ Faça sites responsivos.

✔ Teste em diferentes telas.

✔ Aprenda acessibilidade.

✔ Pense na experiência do usuário (UX).

---

# Exercícios

1. O que é HTML?
2. Qual a função do CSS?
3. Qual a função do JavaScript?
4. Explique Front-End.
5. Explique Back-End.
6. O que é DOM?
7. Crie uma página HTML simples.
8. Adicione CSS.
9. Crie um botão com JavaScript.
10. Explique o conceito Full Stack.

---

# Projeto Prático Final do Capítulo

Crie um site profissional de portfólio.

Deve possuir:

## Página inicial

* Nome;
* Foto;
* Descrição.

## Projetos

* Lista dos seus projetos;
* Links do GitHub.

## Contato

* Formulário;
* Redes sociais.

Tecnologias:

✅ HTML
✅ CSS
✅ JavaScript

Depois publique utilizando GitHub.

---

# Resumo do capítulo

Neste capítulo você aprendeu:

✅ Como funciona a web.
✅ Diferença entre Front-End e Back-End.
✅ O papel do HTML.
✅ O papel do CSS.
✅ O papel do JavaScript.
✅ Estrutura de projetos web.
✅ DOM.
✅ Eventos.
✅ Responsividade.
✅ Ferramentas profissionais.

---

## Próximo capítulo

No **Capítulo 21**, você aprenderá **Git e GitHub na prática para Desenvolvedores**, criando repositórios profissionais, commits, branches, pull requests, README e preparando seu portfólio para o mercado de trabalho.
