# MySQL - trabalhando com tabelas

Created: January 20, 2022 9:31 AM

---

# Primeiros passos na criação de suas tabelas

- Modelo Relacional
    - O modelo relacional surge na década de 60, proposto por Edgar Codd.
    - As tabelas são compostas por entidades, atributos e chaves.
    - As chaves permitem o relacionamento entre os dados.
- Por que usar tabelas?
    - Dados organizados de forma estruturada.
    - Dados atômicos.
    - Consulta e manipulação de dados simplificados.
- Criando a tabela
    - CREATE TABLE
    - Tipos: INT, VARCHAR, DATETIME
    - CREATE TABLE pessoa (nome varchar(20), nascimento date);
- Inserindo dados
    - INSERT INTO
    - Indicar as colunas que serão preenchidas e os respectivos valores.
    - INSERT INTO pessoas (nome, nascimento) VALUES (’Lola’, ‘1990-07-22’);

# Realizando manutenção de suas tabelas

- Selecionando dados
    - SELECT
    - Definindo os campos viualizados
    - SELECT * FROM pessoas
- Atualizando dados
    - UPDATE
    - Alterando informações na tabela
    - UPDATE pessoas SET  nome = ‘Lola’
- Cláusula WHERE
    - WHERE
    - Define uma condição para nosso comando
    - UPDATE pessoas SET nome = ‘Lola’ WHERE = id=1
- Deletando dados
    - DELETE FROM
    - Deleta as informações selecionadas
    - DELETE FROM pessoas WHERE id=1
- Ordenando dados
    - ORDER BY
    - Ordena a forma como as informações são exibidas
    - SELET * FROM  pessoas ORDER BY  nome
- Agrupando
    - GROUP BY
    - Agrupa as informações de acordo com o critério selecionado
    - SELECT COUNT(qtd), GENERO FROM pessoas GROUP BY  genero