# Coleções

Created: January 20, 2022 9:26 AM

---

# Map

`const myMap = new Map()`

- Características:
    - Uma coleção de arrays no formato `[chave, valor]`;
    - Pode ser iterado por um loop for ... of
- Métodos
    - Adicionar
        - `MyMap.set(’apple’, ‘fruit’);`
        - // Map(1) {”apple” ⇒ “fruit”}
    - Ler
        - `MyMap.get(”apple”);`
        - // “fruit”
    - Deletar
        - `MyMap.deleted(”apple”);`
        - // true
    - Retornar o valor
        - `MyMap.get(”apple”);`
        - // undefined

Maps

- Podem ter chaves de qualquer tipo.
- Possuem a propriedade length.
- São mais fáceis de iterar.
- Utilizado quando o valor das chaves é desconhecido.
- Os valores tem o mesmo tipo.

Objeto

- Sempre tem chave no formato string.
- Tem que iterar por todas as propriedades para saber quantas tem.

# Set

`const mySet = new Set();`

- São estruturas que armazenam apenas **valores únicos**, não se repetem nunca.
- Métodos
    - Adicionar
        - `mySet.add(1);`
    - Consultar
        - `mySet.has(1);`
        - // true
    - Deletar
        - `mySet.delete(1);`

Set

- Possui valores únicos.
- Em vez da propriedade length, consulta-se o número de registro pela propriedade *size*;
- Não possui os métodos *map*, *filter*, *reduce*, etc.