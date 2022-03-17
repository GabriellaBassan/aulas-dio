# Manipulando a DOM com JS

Created: January 20, 2022 9:28 AM

---

# Entendendo o D.O.M

- Document Object Model

O DOM HTML é um padrão de como **acessar e modificar os elementos HTML de uma página.**

---

BOM

- Browser Object Model

É tudo o que está dentro do objeto window.

# Selecionando elementos

| Método | Descrição |
| --- | --- |
| document.createElement("element") | Cria um novo elemento HTML |
| document.removeChild(element) | Remove um elemento filho |
| document.appendChild(element) | Adiciona um elemento |
| document.replaceChild(new, old) | Substitui um elemento |

# Trabalhando com estilos

`Element.classList`

- **classList** é o atributo do elemento

```jsx
const meuElemento = document.getElementById("meu-elemento")

meuElemento.classList.add("novo-estilo");
// adiciona a classe "meu estilo"

meuElemento.classList.remove("classe");
// remove classe "classe"

meuElemento.classList.toggle("dark-mode");
// adiciona a classe "drk-mode" caso ela não exista.
// se existir remove da lista
```

---

Para acessar diretamente o CSS de um elemento

- `document.getElementsByTagName("p").style.color = "blue";`

# Eventos

- Tipos:
    - Eventos do mouse
        - mouseover, mouseout
    - Eventos de clique
        - click, dbclick
    - Eventos de atualização
        - change, load

**Event listener**: diretamente no JS, cria um evento que vai ser acionado no momento em que o usuário realizar determinada ação.

```jsx
const botao = document.getElementById("meuBotao");
						 //tipo do evento	|	oq vai ser feito depois que o evento for ativado			
botao.addEventListener("click", outraFuncao);
```

---

Atributo HTML: especifica a função a ser chamada diretamente no elemento HTML.

```html
<h1 onclick="mudaTexto(this)">Clique aqui</h1>

<script>
	function mudaTexto(id) {
		id.innerHTML = "Mudei";
}
</script>
```