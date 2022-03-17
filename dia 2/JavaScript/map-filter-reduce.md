# Map, Filter e Reduce

Created: January 20, 2022 9:28 AM

---

# Map

- Não modifica o array original, o retorno da unção cria um novo array.

Realiza operações em ordem.

`array.map(callback, thisArg)`

- **thisArg(optional)**: valor ‘this’ dentro da função de callback.

`callback(item, index, array)`

- **callback**: função a ser executada em cada elemento.

---

**Map vs forEach**

- valor de retorno é diferente.
- Precisa considerar se o array auxiliar será necessário.

```jsx
// Usando map

const array = [1, 2, 3, 4, 5];
array.map((item) => item * 2); // retorno: [2, 4, 6, 8, 10];

//Usando forEach

const array = [1, 2, 3, 4, 5];
array.forEach((item) => item * 2); // retorno: undefined
```

# Filter

- Não modifica o array original, o retorno uma nova lista apenas com os itens que passaram pelo filter.

Cria um novo array.

`array.filter(callback, thisArg)`

- **thisArg(optional)**: valor ‘this’ dentro da função de callback.
- **callback**: função a ser executada em cada elemento.

---

```jsx
const frutas = ['maçã fuji', 'maçã verde', 'laranja', 'abacaxi'];
frutas.filter((frutas) => fruta.includes('maçã))

//retorno: ['maçã fuji', 'maçã verde'];
```

# Reduce

Executa uma função em todos os elementos do array, retornando um valor único.

`array.reduce(callbackFn, initialValue)`

- **callback**: função a ser executada a partir do acumulador.
- **initialValue**: valor sobre o ****qual o retorno final irá atuar (é opcional).

```jsx
const callbackFn = function(acumulator, currentValue, index, array) {
	// do something
}

array.reduce(callbackFn, initialValue)
```

- **Acumulator/prevValue**: acumulador de todas as chamadas de *callbackFn*.
- **currentValue**: elemento atual sendo acessado pela função.