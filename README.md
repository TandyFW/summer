# O que vamos aprender?

Vamos turbinar nossos conhecimentos em css aprendendo uma nova forma de posicionar nossos elementos na tela com o uso de flexbox.

## Você será capaz de:

*	Utilizar o display flex para definir o elemento “container”.
*	Utilizar a propriedade flex-direction para definir a direção que os elementos dentro do container seguirão.
*	Utilizar align-items, justify-content e align-content para posicionar os elementos dentro do “container”.
*	Utilizar flex-wrap para definir se os elementos se aglomerarão em uma única linha ou coluna ou pularam para a próxima caso exceda o espaço.

### Por que isso é importante?

A construção do layout de uma página pode a ser algo muito desafiador, principalmente torná-lo responsivo para múltiplos tamanhos de telas. Com a ajuda do flexbox é possível criar layouts responsivos com mais facilidade e fluidez devido a forma que os elementos dentro do container flex se ajustam automaticamente de acordo com suas propriedades.

### Conteúdos:

### Display flex

Como já foi visto anteriormente, o display block faz com que os elementos filhos, elementos entre a abertura e o fechamento de uma tag, apareçam verticalmente na tela, um abaixo do outro, enquanto o display inline faz o contrário, fazendo-os aparecer um do lado do outro. O display inline-block faz com que os elementos filhos apareçam um do lado do outro e passem para a linha de baixo antes de chegar na borda do container.

Estes três tipos de display têm outras diferenças não apresentadas acima, caso você queira se aprofundar, acesse os Recursos Adicionais.

A configuração inicial do display flex faz com que os elementos filhos apareçam um do lado do outro, respeitando as margens e adaptando seu width, para caber dentro do elemento pai.

![flex box exemplo 1](/ex1-flexbox-300.jpg)  ![flex box exemplo 2](/ex2-flexbox-300.jpg)

As propriedades que podem ser usadas junto com o elemento container são: flex-direction, flex-wrap, flex-flow, justify-content, align-items e align-content.

### Flex-direction

A propriedade flex-direction define o sentido na qual os elementos serão posicionados. Seguem seus principais valores abaixo:

* row: seu valor default, que faz os elementos filhos ficarem um do lado do outro, iniciando da esquerda para a direita.
* row-reverse: Faz os elementos filhos ficarem um do lado do outro, mas da direita para a esquerda.
* column: Faz os elementos posicionarem-se na vertical, de cima para baixo.
* column-reverse: Faz os elementos posicionarem-se na vertical, de baixo para cima.

Exemplo de código:
````css
.container {
  display: flex;
  flex-direction: column
}
````

Exemplos utilizando os 4 valores acima citados:

![flex box row](/ex3-flexbox-300.jpg)  ![flex box column](/ex4-flexbox-300.jpg)

![flex box row](/ex5-flexbox-300.jpg)  ![flex box column-reverse](/ex6-flexbox-300.jpg)

### Flex-wrap

A propriedade flex-wrap permite que os elementos passem para a próxima linha ou coluna quando alcançar a borda do container. Seguem abaixo seus principais valores:

* nowrap: Valor default, não permite que os elementos filhos mudem de linha ou coluna.
* wrap: Permite que os elementos filhos mudem de linha ou coluna ao alcançarem o padding do container.
* wrap-reverse: Além de permitir que mudem de linha ou coluna faz os elementos começarem na direção reversa.

Exemplo de código:
````css
.container {
  display: flex;
  flex-wrap: wrap;
}
````
Exemplos utilizando wrap e wrap-reverse

display-direction: row

![flex box nowrap](/ex7-flexbox-300.jpg)  ![flex box nowrap](/ex8-flexbox-300.jpg)

display-direction: column

![flex box nowrap](/ex9-flexbox-300.jpg)  ![flex box nowrap](/ex10-flexbox-300.jpg)


