# Sintaxe básica em JS

# JavaScript

É uma linguagem de alto nível, que integra o desenvolvimento de apps e páginas web. É uma das mais usadas no mundo do desenvolvimento.

- Serve para criar scripts dinâmicos que realizam a interação de apps ou páginas web.
- Pode-se usar de várias formas, seu uso mais comum se dá no desenvolvimento de apps e páginas web, juntamente com HTML e CSS.

# Entendendo variáveis e seus valores

A tipagem funciona como uma regra de uso de dados, quanto mais forte for a tipagem, mais obrigatório é a declaração do tipo de dado.

- A tipagem em JavaScript é fraca, a declaração dos dados acontece de modo dinâmico.
    - Ex: Ao criarmos uma variável com *valor* entre *aspas* (`“valor”`) o JavaScript já *converte o dado* para o tipo *String*.
    - Ex: `var numero = 1`; o JavaScript já *converte* o *valor* para o tipo *Number*.

---

As variáveis em JavaScript podem guardar tipos de dados que chamamos de **tipos primitivos.**

- Variáveis podem guardar valores dos tipos:
    
    Para saber o tipo da variável `typeof()`.
    
    - Boolean
    - null
    - undefined
    - Number
    - String
    - Array
    - Object
    - Function

Variáveis são dados que variam. Funcionam como uma caixa que guarda valores.

- Existem 3 modos de declarar as variáveis em JS:
    - **var** – escopo *global e local*, pode ter seu *valor alterado*, se *não tiver* um *valor inicial será tratada como null*;
    - **let** – escopo *local de bloco*, pode ter seu *valor alterado*, se *não tiver um valor inicial será tratada como null*;
    - **const** – escopo *local de bloco*, *somente leitura*, o *valor inicial é obrigatório e não pode ser alterado*.
- O escopo em JavaScript define a limitação e visibilidade de um bloco de código.
    - **Escopo global –** quando a variável é declarada fora de qualquer bloco, sua visibilidade fica disponível em todo o código.
    - **Escopo local –** quando a variável é declarada dentro de um bloco, sua visibilidade pode ficar disponível ou não.
- Regras de uso de variáveis:
    - Iniciar com letras, underscore **_** ou cifrão **$**
    - Não iniciar com número
    - Não usar espaços (use o camelCase ou **_**)
    - Não usar palavras reservadas
    - Declarar variáveis no topo do bloco de código.

---

O sinal de igualdade “**=**“ em JavaScript, significa **atribuição**.

- Ex: como declarar: `var nome = “meu nome”;`
     variável nome recebe o valor meunome

Para fazermos uma **comparação de valores** em JavaScript usamos “**==**“.

- Ex: como declarar: `"0" == 0;` 
     “0” tem o valor igual a 0? // nesse caso retorna true

Para fazermos uma **comparação idêntica de valores e tipos** em JavaScript usamos “**===**“.

- Ex: como declarar: `"0" === 0;` 
     “0” tem o valor e o tipo idêntico a 0? // nesse caso retorna false

---

- Operadores Aritméticos são tipos de operadores matemáticos com valor numérico:
    - adição `+`
    - subtração `-`
    - multiplicação `*`
    - divisão real `/`
    - divisão inteira `%`
    - potenciação `**`
- Operadores Relacionais são tipos de operadores que consultam a relação entre valores:
    - `>` maior que
    - `<` menor que
    - `>=` maior ou igual a
    - `<=` menor ou igual a
- Operadores Lógicos são tipos de operadores que consultam valores lógicos:
    - `&&` - “e” – considera que *todos os valores sejam true*
    - `||` - “ou” – considera que **qualquer valor seja true**
    - `!` - “não” – **inverte o valor de true para false ou vice-versa**

# Vetores e Objetos

Vetores ou Arrays são um tipo de lista, ou matriz de variáveis, onde cada variável possui um índice. Os valores podem ser de vários tipos.

- Um array é uma caixa com várias outras caixas dentro e cada uma contendo algum valor.

O array deve ser declarado entre colchetes “`[]`”, e podem guardar qualquer valor dentro de seus índices: inclusive outros arrays.

- Ex: `let array = ['string', 1, true, false, [‘array1], [‘array2’]...]`
    - Obs.: O índice só é acessado por um número inteiro, onde 0 é o primeiro índice. Cada índice é separado por vírgula.
- Ao ser declarado, o Array traz consigo uma série de métodos para manipulá-lo.
    - `forEach()` – itera um array;
    - `push()` – add item no final do array;
    - `pop()` – remove item no final do array;
    - `shift()` – remove item no início do array;
    - `unshift()` – add item no início do array;
    - `indexOf()` – retorna o índice de um valor;
    - `splice()` – remove ou substitui um item pelo índice;
    - `slice()` – retorna uma parte de um array existente;

---

Objetos são dados que possuem propriedades e valores que definem suas características. Deve ser declarado entre chaves “`{}`”.

```jsx
// Ex: imagine uma xícara azul. 
// Ela tem cor, pode ter vários tamanhos e funções(quero café). 
// Pode ser declarada assim:

var xicara = {
		cor: ‘azul’,
		tamanho: ‘p’,
		funcao: tomarCafe()
}
```

As propriedades de objetos podem ser atribuídas à variáveis, facilitando a manipulação do objeto. Chamamos isso de desestruturação.

```jsx
//Ex: 
var xicara = {cor: ‘azul’, tamanho: ‘p’, funcao: tomarCafe()}

var cor = xicara.cor;
var tamanho = xicara.tamanho;
var funcao = tomarCafe();
```

Outra forma de fazer a desestruturação é utilizando chaves ao
declarar a variável:

```jsx
// Ex:
var xicara = {cor: ‘azul’, tamanho: ‘p’, funcao: tomarCafe()}

var { cor, tamanho, funcao } = xicara;
```

# Estruturas condicionais

São instruções para realizar determinadas tarefas a partir de uma condição, seja de decisão ou repetição.

### Estruturas de decisão

- if
    
    Podemos usar as palavras reservadas “**if**” para estabelecer uma condição:
    
    ```jsx
    // Ex: 
    var jogador1 = 0;
    var jogador2 = 0;
    
    if (jogador1 > 0) {
    console.log(‘jogador1 marcou ponto’);
    }
    // se o jogador1 tiver valor maior que 0 ele marcou ponto.
    ```
    
- else
    
    No caso de a condição não ser atendida podemos usar o “**else**” :
    
    ```jsx
    // Ex: 
    var jogador1 = 1;
    var jogador2 = 0;
    
    if (jogador1 > 0) {
    console.log(‘jogador1 marcou ponto’);
    } else {
    console.log(‘ninguem marcou ponto’);
    }
    ```
    
- else if
    
    Caso haja mais de uma condição usamos o “**else if**“.
    
    ```jsx
    Ex.: var jogador1 = 1;
    var jogador2 = 0;
    
    if (jogador1 > 0) {
    console.log(‘jogador1 marcou ponto’);
    } else if (jogador2 > 0) {
    console.log(‘jogador2 marcou ponto’);
    } else {
    console.log(‘ninguém marcou ponto);
    }
    ```
    
- ninho de if
    
    Podemos também usar o “**if**” dentro de um outro “**if**”, chamamos isso de aninhamento de if’s ou ninho de if’s.
    
    ```jsx
    // Ex: 
    if (jogador1 = -1) {
    			if (jogador1 > 0) {
    						console.log(‘jogador 1 marcou ponto’);
    			} else {
    						console.log(‘ninguém marcou ponto’);
    			}
    		} else {
    				console.log(‘jogador inválido’);
    }
    ```
    
- if ternário
    
    Podemos também fazer uma verificação em uma única linha usando o “**if**” ternário:
    
    ```jsx
    // Ex 
    [condição] ? [instrução1] : [instrução2];
    
    jogador1 > 0 ? console.log(‘marcou ponto’) : console.log(‘não
    marcou ponto”);
    
    // lembre de usar a interrogação “?” e dois pontos “:”
    ```
    
- switch/case
    
    O “**switch/case**” funciona como uma estrutura condicional
    também.
    
    ```jsx
    // Ex: 
    switch (${expressao}) {
    	case 1:
    		${instrucao};
    	break;
    	case 2:
    		${instrução};
    	break;
    }
    // lembre de usar "break" ao final para não ficar em loop infinito
    ```
    

### Estruturas de repetição

São estruturas condicionais que repetem uma instrução até atingir determinada condição:

- for
    
    Funciona como uma repetição de instrução até que a condição seja falsa:
    
    ```jsx
    for ([expressaoInicial]; [condicao]; [incremento]) {
    declaracao }
    
    // Ex: 
    var array = [‘valor1’, ‘valor2’, ‘valor3’, ‘valor4’]
    
    for (let i = 0; i < array.length; i++) {
    console.log(i);
    }
    ```
    
- for/in
    
    Funciona como uma repetição a partir de uma propriedade:
    
    ```jsx
    for ([indice] in [objeto ou array]) {
    declaracao }
    
    // Ex: 
    var array = [‘valor1’, ‘valor2’, ‘valor3’, ‘valor4’]
    
    for (i in array) {
    console.log(i);
    }
    ```
    
- for/of
    
    Funciona como uma repetição a partir de um valor:
    
    ```jsx
    for ([indice] of [array]) {
    declaracao }
    
    // Ex: 
    var array = [‘valor1’, ‘valor2’, ‘valor3’, ‘valor4’]
    
    for (i of array) {
    console.log(i);
    }
    ```
    
    - Não funciona com objetos pois as propriedades variam, diferentes do índice em um array que sempre serão números inteiros.
    
    ```jsx
    // Mas e se eu quiser pegar o valor mesmo assim?
    // Ex: 
    for (i of object.propriedade) {
    console.log(i);
    }
    // porém cada caractere dentro do valor será
    // impresso em linhas separadas.
    ```
    
- while
    
    Executa uma instrução “**enquanto**” determinada condição for verdadeira, a verificação é feita antes da execução.
    
    ```jsx
    // Ex: 
    var a = 0;
    	while (a < 10) {
    		a++;
    		console.log(a);
    }
    // enquanto a variável a for menor que 10 ela
    // vai receber mais um e imprimir no console.
    ```
    
- do/while
    
    Executa uma instrução “**até que**” determinada condição seja falsa, a verificação é feita depois da execução.
    
    ```jsx
    // Ex: 
    var a = 0;
    	do {
    	a++;
    	console.log(a);
    } while (a < 10)
    
    // a variável a vai receber mais um e imprimir
    // no console até que seu valor chegue a 10
    ```
    

# Funções e suas particularidades

São blocos de comandos e instruções para a execução de determinadas tarefas.

- Geralmente se utiliza a palavra reservada “**function**” seguida de parênteses “`()`” e chaves “`{}`”:

```jsx
// Ex: função declarativa
function funcao() { // é obrigatório ter um nome
	console.log(“mensagem”);
}

funcao(); // chamada a função

// () – indica que é um objeto do tipo function;
// {} – indica que é um bloco de instrução;
```

As funções podem receber em sua declaração, **parâmetros**, que **servem** como **variáveis**, onde sua **atribuição pode ser feita durante a chamada da função**:

```jsx
// Ex: 
function nomeDaFuncao(parametro) {
	${instrucao};
}

nomeDaFuncao(valorDoParametro);
```

- Funções atribuídas à **expressões**. A nomeação das funções por expressão é *opcional*:

```jsx
// Ex: 
var funcao = function nomeDaFuncao() {
		${instrucao};
}

//Ex: 
var funcao = function() {
		${instrucao};
};
```

- **Arrow Function** são funções de expressão de sintaxe curta. **Sempre** serão **anônimas**, e portanto não podem ser nomeadas, **deve** ser **declarada com parênteses** "`()`", seguido de "`=>`" e depois chaves "`{}`"

```jsx
// Ex: 
var funcao = () => {
		${instrucao};
}
```