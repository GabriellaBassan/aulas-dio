# Funções

Created: January 20, 2022 9:25 AM

---

# Tipos de Função

- Definição comum de uma função.
    
    ```jsx
    function nome(parametros) {
    	// instruções
    }
    ```
    
    - Variáveis criadas dentro de uma função apenas podem ser utilizadas dentro dela.
    - Quando invocamos o “**return**”, a função **para de ser executada**.
- Função Anônima
    - Funções que representam expressões.
        - Sem nome.
        - Uma variável pode armazenar uma função.
        
        ```jsx
        const soma = function (a, b) {
        	return a + b;
        }
        
        soma (1, 2)
        soma(5, 4)
        ```
        
- Função Autoinvocável
    
    IIFE (Immediately Invoked Function Expression)
    
    - Uma função anônima entre parênteses, seguida por outro par de parênteses, que representa sua chamada.
    
    ```jsx
    (
    	function() {
    		let name = "Lola"
    		return name;
    	}
    )();
    
    // Lola
    ```
    
    - Também pode ser utilizada com parâmetros ou armazenada em uma vaiável.
    
    ```jsx
    (
    	function(a, b) {
    		return a + b;
    	}
    )(1, 2);
    
    ----------------------------------------------
    
    const soma3 = (
    	function() {
    		return a + b;
    	}
    )(1, 2);
    
    console.log(soma3) 
    ```
    
- Callbacks
    - Uma função passada como argumento para outra.
        - Utilizando callbacks, tem maior controle da ordem de chamadas.
        
        ```jsx
        const calc = function(operacao, num1, num2){
        	return operacao(num1, num2);
        }
        
        const soma = function(num1, num2) {
        	return num1 + num2;
        }
        
        const sub = function(num1, num2) {
        	return num1 - num2;
        }
        
        const resultSoma = calc(soma, 1, 2);
        const resultSub = calc(sub, 1, 2);
        
        console.log(resultSoma);
        console.log(resultSub);
        ```
        

# Parâmetros

- Objeto “arguments”
    - Um array com todos os parâmetros passados quando a função foi invocada.
- Arrays
    - **Spread**: uma forma de lidar separadamente com elementos.
        - O que era parte de um array se torna um elemento independente.
        
        ```jsx
        function sum(x, y, z) {
        	return x + y + z;
        }
        
        const numbers = [1, 2, 3];
        
        console.log(sum(...numbers));
        ```
        
    - **Rest**: combina os argumentos em um array.
        - O que era um elemento independete se torna parte de um array.
        
        ```jsx
        function confereTamanho(...args) {
        	console.log(args.length);
        }
        
        confereTamanho();
        confereTamanho(1, 2);
        confereTamanho(3, 4, 5);
        ```
        
- Objetos
    
    Object Destructuring
    
    - Entre chaves, podemos filtrar apenas os dados que nos interessam em um objeto.

# Loops

- Switch/case
    - Equivale a uma comparação de tipo e valor ( `===` )
    - Sempre precisa de um valor “`default`”
    - Ideal para quando se precisa comparar muitos valores.
- For
    - Loop dentro de elementos iteráveis (arrays, strings).
    - For ... in
        - Loop entre propriedades enumeráveis de um objeto.
    - For ... of
        - Loop entre estruturas iteráveis (arrays, strings)
            - A sintaxe mais fácil do que o a do For.
- While
    - Executa instruções até que a condição se torne falsa.
    - Do ... while
        - Executa intruções até que a condição se torne falsa.
        - Porém **a primeira execução sempre ocorre**.

# This

A palavra reservada **this** é uma referência de contexto.

- Seu valor pode mudar de acordo com o lugar no código onde foi chamada.

| Contexto | Referência |
| --- | --- |
| Em um objeto (método) | Próprio objeto dono do método |
| Sozinha | Objeto global (em navegadores, window) |
| Função | Objeto global |
| Evento | Elemento que recebeu o evento. |
- Manipulando o valor
    - Call
        - É possível passar parâmetros para a função separando-os por vírgulas.
    - Apply
        - É possível passar parâmetros para essa função dentro de um array.
    - Bind
        - Clona a estrutura da função onde é chamada e aplicsr o valor do objeto passado como parâmetro.

# Arrow Functions

- Caso exista apenas uma linha, pode dispensar as chaves e o return.

```jsx
const soma = (a, b) => a + b;

soma(4, 6);
```

- Caso exista apenas um parâmetro, pode dispensar os parênteses.

```jsx
const soma = a => a;

soma(4);
```

Arrow function **não** faz hoisting.

- Outras restrições:
    - “this” sempre será o objeto global. Métodos para modificar seu valor não irão funcionar.
    - Não existe o objeto “arguments”.
    - O constructor também não pode ser utilizado.