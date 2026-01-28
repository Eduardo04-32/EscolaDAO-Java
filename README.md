# PROJETO ESCOLA UTILIZANDO DAO - Java + JDBC 

Este projeto foi desenvilvido para demostrar apratica de como funciona a **arquiquetura em camadas** utilizando **Java** e **MySQL**, aplicando o padrão **DAO(Data Acasso Object)**.

O siatema permite cadastrar alunos e listar alunos armazenando em um banco de dados.

---

# Objetivo do projeto 

- Separar responsabilidades no código
- Demostrar a conexão entre Java e Banco de dados
- Aplicar boa praticas como:
- DAO
- Model
- Factory de Conection
- Evitar de SQL Injector
- Facilita a manutenção e evolução do sistema
 ---

 # Estrutura do Projeto

<img width="233" height="199" alt="image" src="https://github.com/user-attachments/assets/573606e9-23f2-446d-bb24-02fa231c8a71" />

## Descrição das camadas 👨‍💻

- Main (app)

- Responsavel por:

- Interagir com o usuario via console

- Receberv dados

- Chamar o DAO para salvar a çista açunos

- Não contem SQL, Apenas agrega o fluxo da aplicação

- Aluno (Model)

- Representar a tabela

- Contém:

-  Atributos (id, nome)

-  Construtores

-  Getter Setter

-  AlunoDAO (dao)

Responsável por:

Executar comandos SQL

Fazer operações CRUD

Converter dados do banco em objetos Java

Métodos:

cadastrar(Aluno aluno)

listar()

- Centraliza toda a lógica de acesso ao banco.

- ConnectionFactory (config)

Responsável por:

Criar e fornecer conexões com o banco de dados

Centralizar URL, usuário e senha

- Facilita manutenção e evita repetição de código.

## Importância do Padrão DAO

O padrão DAO (Data Access Object) é importante porque:

Separa regras de negócio do acesso ao banco

Facilita testes

Permite trocar o banco sem alterar o restante do sistema

Torna o código mais organizado e profissional

É amplamente usado no mercado de trabalho
