# Manipulação de Listas em JS
Costumeiramente, nós, programadores, usamos listas e objetos para armazenar várias informações em uma única variável. Mas se a gente quiser criar variáveis com versões alteradas dessa lista, com dados contextualizados e não brutos? Afinal, como diz o ditado, em um programa, o que vale não é o dado bruto, mas sim esse dado com o contexto certo aplicado a ele. 

Nesse repositório, nós aprenderemos a fazer isso mesmo: A manipulação de listas e objetos em JS, usando os métodos `.map()`, `.filter()` e `.reduce()`.

## Uso de .map() no JS

Comecemos pelo método mais comum entre os três. O método `.map()`, da classe Array, executa uma função de callback (função como parâmetro de outra) a cada elemento de um array. O retorno do callback será direcionado a uma nova lista, que será passada para a variável onde está sendo atribuida o retorno do método `.map()`.
