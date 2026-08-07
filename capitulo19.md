# CURSO COMPLETO DE PROGRAMAÇÃO

# Do Zero ao Desenvolvedor Full Stack

## Volume 2 – Fundamentos da Programação

# CAPÍTULO 19

# Banco de Dados: Armazenando Informações de Sistemas Profissionais

> **Objetivo do capítulo:** Ao final deste capítulo, você entenderá o que são bancos de dados, por que eles são essenciais, como funcionam, conhecerá SQL e NoSQL, aprenderá conceitos como tabelas, registros, relacionamentos e verá como aplicações reais armazenam informações.

---

# Introdução

Até agora aprendemos a criar programas que:

* recebem dados;
* processam informações;
* mostram resultados.

Mas existe um problema:

Quando fechamos o programa, os dados desaparecem.

Exemplo:

Um sistema de login:

```text
Usuário:
Davi

Senha:
123456
```

Se o programa for encerrado, essas informações precisam continuar existindo.

Como resolver?

Utilizando:

# Banco de Dados

---

# O que é um banco de dados?

Um banco de dados é um sistema utilizado para armazenar, organizar e consultar informações.

Ele funciona como uma grande biblioteca digital.

Exemplo:

Uma loja virtual precisa armazenar:

```text
Clientes

Produtos

Pedidos

Pagamentos

Endereços
```

---

# Onde os bancos de dados são usados?

Praticamente em todos os sistemas modernos.

## Redes sociais

Armazenam:

* usuários;
* fotos;
* mensagens;
* comentários.

---

## Jogos online

Armazenam:

* contas;
* progresso;
* inventário;
* ranking.

---

## Bancos

Armazenam:

* clientes;
* saldo;
* transações.

---

## E-commerce

Armazena:

* produtos;
* compras;
* entregas.

---

# Banco de Dados x Arquivo comum

Muitas pessoas começam guardando informações em arquivos.

Exemplo:

```txt
usuarios.txt
```

Conteúdo:

```text
Davi,15
Carlos,20
Maria,18
```

Funciona para pequenos projetos.

Mas existem problemas:

* dificuldade de busca;
* pouca segurança;
* organização ruim;
* problemas com muitos dados.

---

Um banco de dados oferece:

✅ Organização.

✅ Segurança.

✅ Velocidade.

✅ Controle de acesso.

✅ Consultas avançadas.

---

# Como funciona um banco de dados?

Um banco possui:

## Dados

As informações armazenadas.

---

## Estrutura

Como os dados são organizados.

---

## Sistema de gerenciamento

Software responsável pelo controle.

Chamado:

# SGBD

(Sistema Gerenciador de Banco de Dados)

---

# Exemplos de SGBD

## Bancos relacionais:

Oracle Corporation

Microsoft

MySQL

PostgreSQL Global Development Group

---

## Bancos NoSQL:

MongoDB Inc.

Redis Ltd.

---

# Banco de Dados Relacional (SQL)

O modelo relacional organiza informações em:

# Tabelas

Uma tabela possui:

* colunas;
* linhas.

---

Exemplo:

Tabela:

## Usuários

| ID | Nome   | Idade |
| -- | ------ | ----- |
| 1  | Davi   | 15    |
| 2  | Carlos | 20    |
| 3  | Maria  | 18    |

---

# Conceitos importantes

## Tabela

Local onde os dados ficam armazenados.

Exemplo:

```text
usuarios
```

---

## Coluna

Representa uma característica.

Exemplo:

```text
nome

idade

email
```

---

## Linha (Registro)

Representa um item.

Exemplo:

```text
Davi | 15 | email@email.com
```

---

## Campo

É um valor específico.

Exemplo:

```text
Nome = Davi
```

---

# Chave Primária (Primary Key)

É um identificador único.

Exemplo:

Tabela usuários:

| ID | Nome   |
| -- | ------ |
| 1  | Davi   |
| 2  | Carlos |

O ID nunca deve se repetir.

---

# Chave Estrangeira (Foreign Key)

É usada para conectar tabelas.

Exemplo:

Tabela:

## Usuários

```text
id_usuario
nome
```

Tabela:

## Pedidos

```text
id_pedido
id_usuario
produto
```

O pedido sabe qual usuário realizou a compra.

---

# Relacionamentos entre tabelas

Existem três principais:

---

# 1. Um para Um (1:1)

Um registro possui apenas outro relacionado.

Exemplo:

Pessoa:

```text
1 pessoa

1 CPF
```

---

# 2. Um para Muitos (1:N)

Mais comum.

Exemplo:

Um usuário:

```text
1 usuário
```

Pode ter:

```text
vários pedidos
```

---

# 3. Muitos para Muitos (N:N)

Exemplo:

Alunos e cursos.

Um aluno pode fazer vários cursos.

Um curso possui vários alunos.

---

# O que é SQL?

SQL significa:

# Structured Query Language

É uma linguagem usada para conversar com bancos de dados.

Com SQL podemos:

* criar tabelas;
* inserir dados;
* buscar informações;
* alterar dados;
* excluir registros.

---

# Criando uma tabela

Exemplo:

```sql
CREATE TABLE usuarios (

id INT PRIMARY KEY,

nome VARCHAR(100),

idade INT

);
```

---

# Inserindo dados

Comando:

```sql
INSERT INTO usuarios
(nome, idade)

VALUES

('Davi',15);
```

---

# Consultando dados

Comando:

```sql
SELECT * FROM usuarios;
```

Resultado:

```text
Davi
15
```

---

# Filtrando dados

Usamos:

```sql
WHERE
```

Exemplo:

```sql
SELECT *
FROM usuarios
WHERE idade >= 18;
```

Resultado:

Usuários maiores de idade.

---

# Atualizando dados

Comando:

```sql
UPDATE
```

Exemplo:

```sql
UPDATE usuarios

SET idade = 16

WHERE nome='Davi';
```

---

# Excluindo dados

Comando:

```sql
DELETE
```

Exemplo:

```sql
DELETE FROM usuarios

WHERE id=1;
```

---

# Banco de Dados NoSQL

NoSQL significa:

# Not Only SQL

São bancos que não utilizam necessariamente tabelas.

Eles trabalham com:

* documentos;
* objetos;
* chave e valor.

---

# Exemplo MongoDB

Documento:

```json
{
 "nome":"Davi",
 "idade":15,
 "cidade":"Araquari"
}
```

---

# Diferença SQL x NoSQL

| SQL                    | NoSQL              |
| ---------------------- | ------------------ |
| Tabelas                | Documentos         |
| Estrutura fixa         | Estrutura flexível |
| Relacionamentos fortes | Grandes volumes    |
| Dados organizados      | Alta velocidade    |

---

# Quando usar SQL?

Ideal para:

* bancos;
* sistemas empresariais;
* lojas;
* sistemas financeiros.

Exemplos:

* PostgreSQL;
* MySQL;
* SQL Server.

---

# Quando usar NoSQL?

Ideal para:

* redes sociais;
* aplicativos grandes;
* sistemas em tempo real.

Exemplos:

* MongoDB;
* Redis.

---

# Banco de dados e programação

Um sistema completo normalmente possui:

```text
Usuário

↓

Interface

↓

Código

↓

Banco de Dados
```

---

Exemplo:

Login:

Usuário digita:

```text
email
senha
```

Programa:

```text
envia dados
```

Banco:

```text
verifica usuário
```

Retorna:

```text
acesso permitido
```

---

# ORM (Object Relational Mapping)

ORM permite usar banco de dados utilizando objetos da programação.

Exemplo:

Em vez de escrever:

```sql
SELECT * FROM usuarios;
```

Usamos:

```javascript
Usuario.findAll();
```

---

Alguns ORMs:

* Prisma;
* Sequelize;
* Hibernate;
* Entity Framework.

---

# Segurança em bancos de dados

Um programador precisa proteger informações.

Principais cuidados:

## Senhas

Nunca guardar:

```text
senha123
```

O correto:

Usar:

```text
hash
```

---

## SQL Injection

Ataque onde alguém tenta manipular comandos SQL.

Exemplo perigoso:

```sql
SELECT *
FROM usuarios
WHERE nome='entrada_usuario';
```

Deve existir proteção.

---

## Controle de acesso

Nem todo usuário deve acessar tudo.

Exemplo:

Administrador:

```text
pode excluir
```

Usuário comum:

```text
apenas visualizar
```

---

# Backup

Todo sistema profissional precisa de cópias dos dados.

Exemplo:

* backup diário;
* backup automático;
* recuperação de dados.

---

# Projetos que usam banco de dados

## Sistema de ordem de serviço

Tabelas:

```text
Clientes

Equipamentos

Serviços

Pagamentos
```

---

## Loja virtual

Tabelas:

```text
Produtos

Clientes

Pedidos

Estoque
```

---

## Rede social

Tabelas:

```text
Usuários

Postagens

Curtidas

Comentários
```

---

# Boas práticas

✔ Planeje o banco antes de criar.

✔ Use nomes claros.

✔ Evite dados duplicados.

✔ Faça backups.

✔ Proteja informações.

✔ Aprenda SQL mesmo usando ferramentas automáticas.

---

# Exercícios

1. O que é um banco de dados?
2. O que significa SGBD?
3. Qual a diferença entre SQL e NoSQL?
4. O que é uma tabela?
5. O que é uma chave primária?
6. Explique chave estrangeira.
7. O que é SQL?
8. Para que serve SELECT?
9. Para que serve INSERT?
10. Explique a importância da segurança.

---

# Projeto Prático

Crie o banco de dados de uma plataforma de jogos.

Crie tabelas:

## Usuários

```text
id

nome

email

senha
```

## Jogos

```text
id

nome

categoria

nota
```

## Biblioteca

```text
id_usuario

id_jogo

data_compra
```

Faça:

✅ Modelo do banco.
✅ Relacionamentos.
✅ Comandos SQL.
✅ Documentação no GitHub.

---

# Resumo do capítulo

Neste capítulo você aprendeu:

✅ O que são bancos de dados.
✅ Como sistemas armazenam informações.
✅ SGBD.
✅ SQL e NoSQL.
✅ Tabelas, registros e colunas.
✅ Chaves primárias e estrangeiras.
✅ Relacionamentos.
✅ Comandos SQL básicos.
✅ Segurança de dados.
✅ Como bancos fazem parte de aplicações reais.

---

## Próximo capítulo

No **Capítulo 20**, você aprenderá **Desenvolvimento Web: HTML, CSS e JavaScript**, entrando na criação de páginas, interfaces, sites responsivos e aplicações que funcionam diretamente no navegador.
