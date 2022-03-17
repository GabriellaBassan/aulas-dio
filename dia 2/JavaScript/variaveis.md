# Variáveis e tipos

# Atribuindo valores

| Case Type | Example |
| --- | --- |
| Original Variable as String | `some awesome var` |
| Camel Case (muito usada no js) | `someAwesomeVar` |
| Snake Case | `some_awesome_var` |
| Kebab Case | `some-awesome-var` |
| Pascal Case | `SomeAwesomeVar` |
| Upper Case Snake Case (muito usado para const) | `SOME_AWESOME_VAR` |
---
- **var** → faz hoisting, reatribui e redeclara valores, escopo global ou local.
- **let** → não faz hoisting, reatribui, mas e não redeclara valores, escopo de bloco.
- **const** → não faz hoisting, não retribui e não redeclara valores, escopo de bloco.

# Tipos

JS é uma linguagem de tipagem dinâmica, ou seja, antes de declarar um valor, não precisa especificar o **tipo** dele.

- Tipos Primitivos: **não** tem **métodos dentro** deles, são **escritos com letra minúscula**.
    - strings
        - Comumente utilizada para textos.
        - São declarados entre aspas ou crases (template string).
    - numbers
        - Números inteiros ou decimais.
            - `Math.floor` (arredonda o numero para baixo)
            - `Math.ceil` (arredonda o numero para cima)
    - booleans
        - Retorna true ou false.
    - Also Known as Trivial/ Other Data types:
    - null
        - Retorna um valor falso
        - Não foi inicializado, quer que um valor naõ exista
    - empty
        - Retorna um valor falso
        - Declara uma variável sem valor
            - se for **number** foi **0**
    - undefined
        - Retorna um valor falso
        - Não é declarado,
        - Indefinido, sem valor declarado
- Composto/Tipos Não-Primitivos
    - array ou vetores
        - Lista iterável de elementos.
            - push (adiciona um elemento ao final)
            - unshift (adiciona um elemento no começo)
            - pop (tira o ultimo elemento)
            - shift (tira o primeiro elemento)
    - objetos
        - Estrutura tipo **chave e valor**
            
            ```jsx
            let person = {
            		name: 'John'
            		age: 20
            };
            // chaves: name, age
            // valores: john, 20
            ```