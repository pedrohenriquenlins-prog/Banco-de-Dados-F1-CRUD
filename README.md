# 🏎️ Sistema de Banco de Dados — Fórmula 1

Projeto acadêmico desenvolvido em **MySQL**, com o objetivo de criar e gerenciar um banco de dados relacional inspirado no universo da Fórmula 1.

O sistema permite organizar informações sobre países, equipes, pilotos, Grandes Prêmios e participantes das corridas, utilizando comandos SQL para manipulação e consulta dos dados.

## 🎯 Objetivo do Projeto

Desenvolver e estruturar um banco de dados relacional, aplicando conceitos fundamentais de SQL, como criação de tabelas, relacionamentos, chaves primárias, chaves estrangeiras, inserção, atualização, exclusão e consultas de dados.

## 🛠️ Tecnologias Utilizadas

![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-4479A1?style=for-the-badge&logo=databricks&logoColor=white)

- MySQL
- SQL (DDL e DML)
- MySQL Workbench (ambiente de execução sugerido)

## 🗄️ Estrutura do Banco de Dados

O banco de dados utilizado no projeto é chamado `maquin_f1` e possui cinco tabelas principais:

| Tabela | Descrição |
|---|---|
| `tb_paises` | Armazena os países cadastrados. |
| `tb_equipes` | Armazena as equipes e seus países de origem. |
| `tb_pilotos` | Armazena os pilotos, seus países e equipes. |
| `tb_corridas` | Armazena os Grandes Prêmios e a quantidade de voltas. |
| `tb_participantes` | Relaciona pilotos às corridas e suas posições de largada. |

### 🔗 Relacionamentos

- Um país pode estar relacionado a várias equipes.
- Um país pode estar relacionado a vários pilotos.
- Uma equipe pode possuir vários pilotos.
- Um país pode sediar várias corridas.
- Uma corrida pode possuir vários participantes.
- Um piloto pode participar de várias corridas.

A tabela `tb_participantes` utiliza uma chave primária composta por `sigla_gp` e `num_piloto`.

## ⚙️ Funcionalidades e Operações SQL

O projeto trabalha com diferentes operações de manipulação e consulta de dados:

- **CREATE:** criação do banco de dados e das tabelas.
- **INSERT:** cadastro de países, equipes, pilotos, corridas e participantes.
- **ALTER TABLE:** alteração da estrutura das tabelas, incluindo a adição do campo de salário dos pilotos.
- **UPDATE:** atualização dos salários cadastrados.
- **SELECT:** consulta e recuperação de informações.
- **WHERE e LIKE:** filtragem de registros.
- **IN:** seleção de dados com múltiplas condições.
- **GROUP BY e AVG:** agrupamento e cálculo de médias salariais.
- **ORDER BY:** ordenação dos resultados.
- **DISTINCT:** consulta de valores sem repetição.

## ▶️ Como Executar o Projeto

1. Instale o [MySQL](https://dev.mysql.com/downloads/) e, se desejar, o MySQL Workbench.
2. Clone este repositório:

```bash
git clone https://github.com/SEU-USUARIO/DB_Formula1.git
```

3. Abra o MySQL Workbench.
4. Abra o arquivo `DB_Formula1.sql`.
5. Execute o script SQL.
6. O banco de dados `maquin_f1` será criado com suas tabelas e dados de exemplo.

## 📁 Estrutura do Repositório

```text
DB_Formula1/
│
├── DB_Formula1.sql
└── README.md
```

## 📚 Conhecimentos Desenvolvidos

- Modelagem de banco de dados relacionais.
- Criação e estruturação de tabelas.
- Chaves primárias e estrangeiras.
- Relacionamentos entre tabelas.
- Manipulação e atualização de registros.
- Consultas SQL e filtragem de informações.
- Funções de agregação e agrupamento de dados.

## 👨‍💻 Autor

**Pedro Henrique do Nascimento Lins**

Estudante de Ciência da Computação na UDF, interessado em desenvolvimento de software, tecnologia e bancos de dados.

- GitHub: [@pedrohenriquenlins-prog](https://github.com/pedrohenriquenlins-prog)

---

*Projeto acadêmico desenvolvido para fins de aprendizado e prática de SQL e modelagem de bancos de dados.*
