# Estruturas de dados e algoritmos

# Conceitos iniciais sobre estrutura de dados, arrays e registro

> Estrutura de Dados é uma estrutura organizada de dados na memória de um computador ou em qualquer dispositivo de armazenamento, de forma que os dados possam ser utilizados de forma correta.
> 

Usando as estruturas adequadas através de algoritmos, podemos trabalhar com uma grande/pequena quantidade de dados, como aplicações em bancos de dados ou serviços de busca.

- Conjunto de operações básicas em estruturas de dados.
    - Inserir dados
    - Excluir dados
    - Localizar um elemento
    - Percorrer todos os itens constituintes da estrutura para visualização
    - Classificar, que se resume em colocar os itens de dados em uma determinada ordem (numérica, alfabética, etc)
- Principais Estruturas de Dados
    - Vetores e Matrizes (Arrays)
        - São estruturas de dados simples que podem auxiliar quando há muitas variáveis do mesmo tipo em um algoritmo.
        - Array uni-dimensional é uma variável que armazena várias variáveis do mesmo tipo.
        - O vetor é uma estrutura de dados indexada, que pode armazenar uma determinada quantidade de valores do mesmo tipo.
        - Possuem tamanho fixo.
    - Registro
        - É uma estrutura que fornece um formato especializado para armazenar informações em memória.
        - Nos permite armazenar mais de um tipo de dado.
        - É composto por campos que especificam cada uma das informações que o compõem.
        - Toda estrutura de registro tem um nome (ex: livro), e seus campos podem ser acessados por meio do uso do operador ponto `(.)`. Por exemplo, para acessar o preço de um livro, seria assim: `livro.preco`
    - Lista
        - Armazena dados de um determinado tipo em uma ordem especifica.
        - Possuem um tamanho ajustável
        - Dois tipos:
            - Ligadas
                - Existem os nós onde cada um conhece o valor que está sendo armazenado em seu interior além de conhecer o elemento posterior a ele: por isso ela é chamada de “lista ligada”, pois os nós são amarrados com essa indicação de qual é o próximo nó.
            - Duplamente Ligadas
                - São biderecionais. Os nós sabem quem é o próximo elemento e também quem é o elemento anterior, o que permite a navegação reversa.
    - Pilha
        - Serve como uma coleção de elementos, e permite o acesso a somente um item de dados armazenado.
        - O acesso aos itens é restrito - somente uma vez um item pode ser lido ou removido por vez.
        - Tipos:
            - LIFO ou UEPS
                - Last In First Out, apresenta o critério de: o primeiro elemento a ser retirado é o último que tiver sido inserido.
            - FIFO ou PEPS
                - First In First Out, apresenta o critério de: o primeiro elemento a ser retirado é o primeiro que tiver sido inserido.
    - Fila
        - Admite remoção de elementos e inserção de novos sujeitos à seguinte regra de operação:
            - O elemento removido é oq ue está na estrutura há mais tempo ou seja, o primeiro objeto inserido na fila é também o primeiro a ser removido
    - Árvore
        - Organiza seus elementos de forma hierárquica, onde existe um elemento que fica no topo da árvore, chamado de raiz e existem os elementos subordinados a ele, que são chamados de nós ou folhas.
    - Tabela Hash
        - De dispersão ou espalhamento é uma estrutura de dados especial, que associa chaves de pesquisa a valores.
        - Uma tabela hash é uma generalização da idéia de array, porém utiliza uma função denominada Hashing para espalhar os elementos, fazendo com que os mesmos fiquem de forma não ordenada dentro do mesmo “array” que define a tabela.
        - Permite a associação de “valores” a “chaves”
            - Valores são a posição ou índice onde o elemento se encontra
            - Chave é a parte da informação que compõe o elemento a ser manipulado.
    - Grafos
        - Estruturas que permitem programar a relação entre objetos.
            - Os objetos são vértices ou “nós” do grafo.
            - Os relacionamentos são arestas (a ligação)