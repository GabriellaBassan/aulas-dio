# Debbuging e Error Handling

Created: January 20, 2022 9:26 AM

---

# Tipos de erros

**ECMAScript Error**: erros que ocorrem em tempo de execução. Composto por:

- Mensagem
- Nome
- Linha
- Call Stack

**DOMException**: erros relacionados ao Document Object Model (DOM), são erros referentes a estrutura da árvore de elementos dentro da página da web.

# Criando erros

**Objeto Error**

```jsx
new Error(message, fileName, lineNumber)
// todos os parâmetros são opcionais

const MeuErro = new Error('Mensagem Inválida');

throw MeuErro;

--------------------------------------------------
// dando nome para o erro
const MeuErro = new Error('Mensagem Inválida');
MeuErro.name = 'InvalidMessage';

throw MeuErro;
```