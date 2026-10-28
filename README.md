# Módulo 26 — Introdução ao PostgreSQL

## Objetivo

Pesquisar sobre o PostgreSQL, compreender sua finalidade e registrar minha experiência inicial com a configuração e o acesso a um banco de dados.

## O que é PostgreSQL?

O PostgreSQL é um sistema gerenciador de banco de dados relacional e de código aberto. Ele permite armazenar, organizar, consultar e modificar dados utilizando a linguagem SQL (*Structured Query Language*).

Os dados podem ser organizados em bancos de dados, schemas e tabelas, compostas por linhas e colunas. Também é possível definir regras para manter a integridade das informações, como chaves primárias, restrições e relacionamentos entre tabelas.

Por ser gratuito, multiplataforma e oferecer recursos para aplicações de diferentes tamanhos, o PostgreSQL é uma ferramenta relevante para quem está aprendendo desenvolvimento de software e trabalhando com o back-end.

## Principais características

- **Código aberto:** pode ser utilizado sem custo de licença.
- **Utilização de SQL:** permite criar tabelas, inserir registros, consultar e atualizar informações.
- **Integridade dos dados:** oferece recursos para definir regras e manter os dados consistentes.
- **Relacionamentos:** possibilita relacionar informações armazenadas em diferentes tabelas.
- **Extensibilidade:** oferece recursos adicionais para atender a diferentes necessidades de desenvolvimento.

## Tecnologias utilizadas na prática

Durante esta atividade, configurei um ambiente de estudo utilizando:

- **Linux Mint:** sistema operacional da máquina virtual.
- **Docker:** utilizado para executar os serviços em contêineres.
- **Docker Compose:** utilizado para configurar e iniciar os serviços.
- **PostgreSQL:** sistema gerenciador do banco de dados.
- **pgAdmin 4:** ferramenta gráfica acessada pelo navegador para administrar o PostgreSQL.

Criei o banco de dados `estudos` e configurei a conexão entre o pgAdmin 4 e o PostgreSQL. Com o ambiente funcionando, pude acessar a estrutura do banco, visualizar o schema `public` e trabalhar com comandos SQL.

## Exemplo de SQL

O comando abaixo demonstra como criar uma tabela simples chamada `teste`:

```sql
CREATE TABLE teste (
    id SERIAL PRIMARY KEY,
    nome VARCHAR(100)
);
```

Nesse exemplo, a coluna `id` utiliza `SERIAL` para gerar identificadores numéricos automaticamente, enquanto `PRIMARY KEY` define a chave primária da tabela. A coluna `nome` armazena textos de até 100 caracteres.

## Minha opinião sobre a experiência

Achei o PostgreSQL interessante e intuitivo para começar a estudar bancos de dados. A possibilidade de configurar o ambiente no Linux utilizando comandos e Docker tornou o processo prático. Depois de configurar os serviços e a conexão, consegui acessar e administrar o banco de dados diretamente pelo navegador, utilizando o pgAdmin 4.

Gostei de perceber que não preciso depender exclusivamente de uma interface gráfica para trabalhar com o banco: posso utilizar comandos para configurar o ambiente e SQL para criar e manipular estruturas e dados.

Ainda estou no início do aprendizado de bancos de dados, então pretendo aprofundar meus conhecimentos em consultas SQL, relacionamentos entre tabelas e integração do PostgreSQL com aplicações Java.

Considero essa experiência importante para minha formação como desenvolvedor Full Stack Java, pois compreender como os dados são armazenados e manipulados é fundamental para construir aplicações de back-end.

## Referências

- [Site oficial do PostgreSQL](https://www.postgresql.org/)
- [Documentação oficial — Introdução ao PostgreSQL](https://www.postgresql.org/docs/current/tutorial.html)
- [Documentação oficial do Docker para PostgreSQL](https://docs.docker.com/guides/postgresql/)

---

**Curso:** Desenvolvedor Full Stack Java  
**Módulo:** 26 — Introdução a bancos de dados e PostgreSQL
