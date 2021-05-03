# O que vamos aprender?

Vamos turbinar nossos conhecimentos em css aprendendo uma nova forma de posicionar nossos elementos na tela com o uso de flexbox.

# Você será capaz de:

*	Utilizar o display flex para definir o elemento **container**.
*	Utilizar a propriedade flex-direction para definir a direção que os elementos filhos dentro do container se posicionarão.
*	Utilizar flex-wrap para definir se os elementos filhos se manterão em uma única linha ou coluna ou pularam para a próxima caso exceda o espaço do container.
*	Utilizar flex-flow para definir tanto direction quanto wrap em uma única linha.
*	Utilizar justify-content, align-items e align-content para posicionar os elementos filhos dentro do container de várias formas.

# Por que isso é importante?

A construção do layout de uma página pode a ser algo muito desafiador, principalmente torná-lo responsivo para múltiplos tamanhos de telas. Com a ajuda do flexbox é possível criar layouts responsivos com mais facilidade e fluidez devido a forma que os elementos dentro do container flex se ajustam automaticamente de acordo com suas propriedades.

# Conteúdos:

### Display flex

Como já foi visto anteriormente, o display block faz com que os elementos filhos, elementos entre a abertura e o fechamento de uma tag, apareçam verticalmente na tela, um abaixo do outro, enquanto o display inline faz o contrário, fazendo-os aparecer um do lado do outro. O display inline-block faz com que os elementos filhos apareçam um do lado do outro e passem para a linha de baixo antes de chegar na borda do container.

Estes três tipos de display têm outras diferenças não apresentadas acima, caso você queira se aprofundar, acesse os Recursos Adicionais.

A configuração inicial do display flex faz com que os elementos filhos apareçam um do lado do outro, respeitando as margens e adaptando seu width, para caber dentro do elemento pai.

![flexbox exemplo 1](/ex1-flexbox-300.jpg)  ![flexbox exemplo 2](/ex2-flexbox-300.jpg)

As propriedades que podem ser usadas junto com o elemento container são: flex-direction, flex-wrap, flex-flow, justify-content, align-items e align-content.

### Flex-direction

A propriedade flex-direction define o sentido na qual os elementos serão posicionados. Seguem seus principais valores abaixo:

* row: Seu valor default, que faz os elementos filhos ficarem um do lado do outro, iniciando da esquerda para a direita.
* row-reverse: Faz os elementos filhos ficarem um do lado do outro, mas da direita para a esquerda.
* column: Faz os elementos posicionarem-se na vertical, de cima para baixo.
* column-reverse: Faz os elementos posicionarem-se na vertical, de baixo para cima.

Exemplo de código:
````css
.container {
  display: flex;
  flex-direction: column;
}
````

Exemplos utilizando os 4 valores acima citados:

![flexbox row](/ex3-flexbox-300.jpg)  ![flexbox column](/ex4-flexbox-300.jpg)

![flexbox row](/ex5-flexbox-300.jpg)  ![flexbox column-reverse](/ex6-flexbox-300.jpg)

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

flex-direction: row -> wrap e wrap-reverse

![flexbox nowrap](/ex7-flexbox-300.jpg)  ![flexbox nowrap](/ex8-flexbox-300.jpg)

flex-direction: column -> wrap e wrap-reverse

![flexbox nowrap](/ex9-flexbox-300.jpg)  ![flexbox nowrap](/ex10-flexbox-300.jpg)

### Flex-flow

Flex-flow é um atalho para utilizar flex-direction e flex-wrap juntos em uma única linha.

Exemplo de código:
````css
.container {
  display: flex;
  flex-flow: column-reverse wrap;
}
````

### Justify-content, align-items e align-content

Antes de falar sobre essas três propriedades, você precisa saber a diferença entre main-axis, eixo principal e cross-axis, eixo transversal. O eixo principal é definido pela direção escolhida pelo flex-direction, ou seja, se for row, o eixo principal será horizontal, se for column, será vertical. Já o eixo transversal será o oposto do eixo principal.

![row direction](/row.jpg) ![column direction](/column.jpg)

A propriedade justify-content permite alinhar os elementos filhos de acordo com o eixo principal. Seguem alguns dos principais valores dessa propriedade:

* flex-start: Valor default, faz o alinhamento no sentido padrão da direção escolhida, fazendo os elementos filhos começarem a partir da esquerda no caso de direction: row e de cima no caso de direction: column.
* flex-end: Faz o alinhamento inverso da direção escolhida.
* center: Centraliza os elementos filhos.
* space-around: Põe um espaço igual entre as bordas do container e o primeiro e último elemento, e põe espaços iguais entre os demais elementos.
* space-between: O primeiro elemento filho posiciona-se no ínicio do container e o último elemento no final do container, os demais ficarão espaçados igualmente entre si.
* space-evenly: Põe espaços iguais entre os elementos e a borda do container.
* stretch: Faz os elementos filhos prencherem todo o espaço do container no sentido transversal, este valor vem como default assim como o flex-start quando os elementos filhos não possuem height ou possuem apenas min-height.

Exemplo de código:
````css
.container {
  display: flex;
  justify-content: space-around;
}
````

Exemplos utilizando os valores de justify-content vistos acima:

![flexbox flex-start](/ex11-flexbox-300.jpg)  ![flexbox flex-start](/ex12-flexbox-300.jpg)  ![flexbox flex-start](/ex16-flexbox-300.jpg)

![flexbox flex-start](/ex14-flexbox-300.jpg)  ![flexbox flex-start](/ex15-flexbox-300.jpg)  ![flexbox flex-start](/ex13-flexbox-300.jpg)

![flexbox stretch](/ex17-flexbox-300.JPG)

A propriedade align-items permite alinhar os elementos filhos no sentido do eixo transversal.

* flex-start: Valor default, faz o alinhamento no sentido transversal de cima para baixo, caso a direção seja row e da esquerda para a direita, caso a direção seja column.
* flex-end: Faz o alinhamento transversal contrário, de baixo para cima, caso a direção seja row e da direita para a esquerda caso a direção seja column.
* center: Centraliza os elementos filhos no eixo transversal.
* stretch: Faz os elementos filhos prencherem todo o espaço do container no sentido transversal, caso os elementos não possuam height definida.

Exemplo de código:
````css
.contaier {
  display:flex;
  align-items: flex-end;
}
````

flex-direction: row;

![flexbox flex-start](/ex11-flexbox-300.jpg)  ![flexbox flex-end](/ex18-flexbox-300.JPG)

![flexbox center](/ex19-flexbox-300.JPG)  ![flexbox stretch](/ex17-flexbox-300.JPG)

flex-direction: column;

![flexbox flex-start](/ex20-flexbox-300.JPG)  ![flexbox flex-end](/ex21-flexbox-300.JPG)

![flexbox center](/ex22-flexbox-300.JPG)  ![flexbox stretch](/ex23-flexbox-300.JPG)


