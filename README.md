# Manipulação de Listas em JS
Costumeiramente, nós, programadores, usamos listas para armazenar várias informações em uma única variável. Mas se a gente quiser criar variáveis com versões alteradas dessa lista, com dados contextualizados e não brutos? Afinal, como diz o ditado, em um programa, o que vale não é o dado bruto, mas sim esse dado com o contexto certo aplicado a ele. 

Nesse repositório, nós aprenderemos a fazer isso mesmo: A manipulação de listas em JS, usando os métodos `.map()`, `.filter()` e `.reduce()`.

## Uso de .map() no JS

Comecemos pelo método mais comum entre os três. O método `.map()`, da classe Array, executa uma função de callback (função como parâmetro de outra) a cada elemento de um array. O retorno do callback será direcionado a uma nova lista, que será passada para a variável onde está sendo atribuida o retorno do método `.map()`.

Aqui vai um exemplo do `.map()` sendo usado em uma lista:

```
const datas = ["2026-02-02", "2026-03-10", "2026-04-06"]

datas_em_pt_br = datas.map((data) => {
  resultado = data.split("-")
  return `${resultado[2]}/${resultado[1]}/${resultado[0]}`
})

// Console:
// [ '02/02/2026', '10/03/2026', '06/04/2026' ]
```

## Uso de .filter() no JS

O próximo da lista será o `.filter()`. Esse método torna-se bem útil para encontrar registros específicos em listas. Ele também recebe uma função de callback, mas, desta vez, ele não modifica nada nos itens específicos. Ele serve para selecionar itens de uma lista e criar uma nova lista com esses itens selecionados, em outras palavras, filtrar a lista, como diz o nome da função.

Aqui vai um exemplo de uso:

```
const datas_lista = ["2025-10-07", "2025-11-04", "2026-02-02", "2026-03-10", "2026-04-06"]

datas_apos_2025 = datas_lista.filter((data) => {
  resultado = data.split("-")
  ano = parseInt(resultado[0], 10)
  return ano > 2025; 
})

```
