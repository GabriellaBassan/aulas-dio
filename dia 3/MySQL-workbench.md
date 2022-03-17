# MySQL - Explorando relacionamentos com workbench

Created: January 20, 2022 9:38 AM

---

# Modelo Relacional

- Relaciona informações entre várias tabelas
    - As chaves estrangeiras (Foreign Key) permitem o relacionamento das tabelas.
- Atomiza as informações

---

INNER JOIN

- Permite a mescla entre tabelas

`SELECT * FROM pessoas JOIN cursos ON pessoas.fk_cursos = cursos.id_cursos`