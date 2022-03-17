# Orientação a objetos

Created: January 20, 2022 9:27 AM

---

# Compreendendo Orientação a Objetos

> Existem dois paradigmas na programação:
> 
> 
> 1. Imperative
> 
> 1. Foca em como vai ser resolvido o problema.
> 
> 2. Declarative
> 
> 1. O que vai ser feito.
- Orientação a objetos é *Imperative.*

Os programas são “objetos” que possuem uma série de propriedades.

- Pilares:
    - Herança
        - O objeto filho herda propriedades e métodos do objeto pai.
    - Polimorfismo
        - Objetos podem herdar a mesma classe pai, mas se comportam de forma diferente quando invocamos seus métodos.
    - Encapsulamento
        - Cada classe tem propriedades e métodos independentes do restante do código.
    - Abstração
        - Basicamente simplificar e abstrair cada vez mais.
        
        “Processo mental que consist em isolar um aspecto determinado de um estado de coisas relativamente complexo, a fim de simplificar a sua avaliação ou para permitir a comunicação do mesmo.”
        

# Orientação a Objetos em JavaScript

**Protótipos**: todos os objetos JS herdam propriedades e métodos de um prototype.

- O objeto *Object.prototype* está no topo desta cadeia.

**Classes**: 

- **Syntatic sugar** uma sintaxe feita para facilitar a escrita.

O JS não possui classes nativamente. Todas as classes são objetos e a herança se dá por protótipos.