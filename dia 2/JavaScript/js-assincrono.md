# JavaScript Assíncrono

Created: January 20, 2022 9:27 AM

---

# Assincronicidade

“Que não ocorre ou não se efetiva ao mesmo tempo.”

- O JS roda de maneira síncrona.

**Promises**: objeto de processamento assíncrono. Inicialmente, seu valor é desconhecido. ela pode, então ser **resolvida** ou **rejeitada**.

- Possui 3 estados:
    - Pending
    - Fulfilled
    - Rejected

```jsx
// estrutura Promise
const myPromise = new Promise((resolve, reject) => {
	window.setTimeout(() => {
		resolve(console.log('Resolvida!'));
	}, 2000);
});
```

**Async/await**: ****funções assíncronas precisam dessas duas palavras chave. *Sempre* que quiser o resultado da *promise* precisa colocar *await.*

- Pode utilizar o try ... catch

# Consumindo APIs

- **APIs**: Application Programming Interface.

Uma API é uma forma de intermediar os resultados do back-end com o que é apresentado no front-end. Consegue acessá-la por meio de URLs.

É muito comum que APIs retornem seus dados no formato .json, portanto precisamos tratar esses dados quando os recebermos.

- **fetch**
    - Precisa utilizar o await

```jsx
fetch(url, options)
	.then(response => response.json())
	.then(json => console.log(json))
// retorna uma Promise
```

Operações no banco:

- POST
- GET
- PUT
- DELETE