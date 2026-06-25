# Sistema de Gerenciamento de Biblioteca

## Descrição do Projeto

O Sistema de Gerenciamento de Biblioteca foi desenvolvido com o objetivo de aplicar conceitos de Programação Orientada a Objetos (POO), Modelagem de Banco de Dados Relacional e Persistência de Dados utilizando PostgreSQL.

O sistema permite o gerenciamento completo de bibliotecas, usuários, livros e empréstimos, simulando operações reais de controle de acervo, empréstimo e devolução de exemplares.

O projeto foi desenvolvido para fins acadêmicos, visando integrar conceitos estudados ao longo da disciplina de Desenvolvimento de Sistemas.

---

## Objetivos

Desenvolver uma aplicação capaz de:

* Gerenciar bibliotecas e seus acervos;
* Cadastrar e controlar usuários;
* Realizar empréstimos e devoluções de livros;
* Garantir integridade dos dados por meio de regras de negócio;
* Aplicar conceitos de Programação Orientada a Objetos;
* Implementar um banco de dados relacional normalizado;
* Utilizar relacionamentos entre entidades através de chaves estrangeiras.

---

## Funcionalidades Implementadas

### Gestão de Bibliotecas

* Cadastro de bibliotecas;
* Registro de nome, endereço e telefone;
* Associação de livros ao acervo da biblioteca.

### Gestão de Livros

* Cadastro de livros;
* Registro de título, autor, gênero e quantidade de páginas;
* Controle automático de disponibilidade;
* Associação de livros a uma biblioteca.

### Gestão de Usuários

* Cadastro de usuários;
* Registro de CPF, telefone e e-mail;
* Controle de data de cadastro;
* Identificação única por CPF.

### Gestão de Empréstimos

* Registro de empréstimos;
* Controle de data de empréstimo;
* Definição da data prevista para devolução;
* Registro da devolução efetiva;
* Histórico completo de empréstimos;
* Controle do status do empréstimo.

### Consultas

* Consulta de livros por gênero;
* Consulta de livros por autor;
* Consulta por faixa de páginas;
* Consulta de empréstimos ativos;
* Consulta de histórico de empréstimos.

---

## Modelagem Orientada a Objetos

O sistema foi estruturado em quatro entidades principais:

### Biblioteca

Representa a unidade responsável pelo armazenamento dos livros.

#### Principais atributos

* idBiblioteca
* nome
* endereco
* telefone

#### Relacionamentos

* Uma biblioteca possui vários livros;
* Uma biblioteca participa de vários empréstimos.

---

### Livro

Representa um exemplar disponível para empréstimo.

#### Principais atributos

* idLivro
* titulo
* autor
* genero
* numeroPaginas
* status

#### Relacionamentos

* Pertence a uma biblioteca;
* Pode participar de diversos empréstimos ao longo do tempo.

---

### Usuario

Representa os leitores cadastrados no sistema.

#### Principais atributos

* idUsuario
* nome
* cpf
* email
* telefone
* dataCadastro

#### Relacionamentos

* Pode realizar diversos empréstimos.

---

### Emprestimo

Representa a movimentação de retirada e devolução de livros.

#### Principais atributos

* idEmprestimo
* dataEmprestimo
* dataPrevistaDevolucao
* dataDevolucao
* statusEmprestimo

#### Relacionamentos

* Associado a um usuário;
* Associado a um livro;
* Associado a uma biblioteca.

---

## Regras de Negócio

O sistema implementa as seguintes regras:

### Disponibilidade do Livro

Um livro somente poderá ser emprestado quando estiver com status "Disponível".

Ao registrar um empréstimo:

* status = Emprestado

Ao registrar uma devolução:

* status = Disponível

---

### Controle de Empréstimos

* Um empréstimo deve possuir usuário, livro e biblioteca válidos;
* A data de devolução não pode ser anterior à data de empréstimo;
* O sistema mantém o histórico de empréstimos realizados.

---

### Integridade dos Dados

* CPF único para cada usuário;
* E-mail único para cada usuário;
* Identificação única para todas as entidades;
* Uso de chaves estrangeiras para garantir relacionamentos válidos.

---

## Banco de Dados

O banco de dados foi desenvolvido utilizando PostgreSQL.

### Estrutura de Tabelas

#### biblioteca

Armazena os dados das bibliotecas cadastradas.

#### usuario

Armazena os dados dos usuários do sistema.

#### livro

Armazena os dados dos livros disponíveis.

#### emprestimo

Armazena todo o histórico de empréstimos e devoluções.

---

## Modelo Relacional

### Relacionamentos

Biblioteca (1) → (N) Livro

Usuario (1) → (N) Emprestimo

Livro (1) → (N) Emprestimo

Biblioteca (1) → (N) Emprestimo

---

## Tecnologias Utilizadas

### Linguagem

* Java

### Banco de Dados

* PostgreSQL

### Paradigmas e Conceitos

* Programação Orientada a Objetos (POO)
* Encapsulamento
* Associações entre classes
* Integridade Referencial
* Modelagem Entidade-Relacionamento
* Banco de Dados Relacional

### Ferramentas

* Eclipse IDE
* PostgreSQL
* Git e GitHub
* Excalidraw (Modelagem)

---

## Estrutura do Projeto

```text
ProjetoBiblioteca
│
├── src
│   ├── entidade
│   │   ├── Biblioteca.java
│   │   ├── Livro.java
│   │   ├── Usuario.java
│   │   └── Emprestimo.java
│   │
│   └── main
│       └── App.java
│
├── trabalho BN.sql
├── excalidraw.png
└── README.md
```

---

## Aprendizados Obtidos

Durante o desenvolvimento do projeto foram aplicados conhecimentos relacionados a:

* Criação de classes e objetos;
* Relacionamentos entre entidades;
* Encapsulamento e organização do código;
* Construção de banco de dados relacionais;
* Utilização de chaves primárias e estrangeiras;
* Criação de regras de integridade;
* Modelagem de sistemas orientados a objetos.

---

## Considerações Finais

O Sistema de Gerenciamento de Biblioteca representa a evolução dos conteúdos estudados ao longo do semestre, integrando conceitos de desenvolvimento orientado a objetos e banco de dados.

O projeto demonstra a implementação de um sistema capaz de controlar acervos, usuários e empréstimos de forma organizada, segura e consistente, aproximando-se das práticas utilizadas em aplicações reais.

---

## Autor

Projeto desenvolvido para fins acadêmicos na disciplina de Desenvolvimento de Sistemas.
