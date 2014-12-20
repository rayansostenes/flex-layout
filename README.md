Flex Layout
===========
Um micro-framework css para trabalhar com a especificação flexbox

Exemplo de uso:
```html
<div class="flex-layout horizontal justified">
    <div>1</div>
    <div class="flex">2</div>
    <div>3</div>
</div>
```


Propriedades do Container
-------------------------
![Container](http://css-tricks.com/wp-content/uploads/2014/05/flex-container.svg)

###Classe `.flex-layout`
Essa classe define um flex container, por padrão é definido como `block` mas caso se adicione a classe `.inline`, ele será definido como um elemento `inline`.
*Note que a classe `.flex-layout` por si só não tem nenhum efeito, você deve definir também a direção do fluxo, como descrito abaixo.*

###flex-direction
Estabelece como os elementos serão exibidos dentro do container, e define o eixo principal
deste. Adicione opções de classes à seguir:

* `.horizontal`: Da esquerda pra direita em `ltr`; Da Da direita pra esquerda em `rtl`  
* `.horizontal.reverse`: Da direita pra esquerda em `ltr`; Da esquerda pra direita em `rtl`
* `.vertical` : De cima pra baixo
* `.vertical.reverse` : De baixo pra cima

![Flex-Direction](http://css-tricks.com/wp-content/uploads/2014/05/flex-direction1.svg)


###flex-wrap
Por padrão, os itens dentro de um flex container vão tentar se acondicionar em uma unica linha. Para alterar este comportamento e permitir que os itens se acondicionem em varias linhas adicione as classes `.wrap` ou `.wrap-reverse` no seu container.

![flex-wrap](http://css-tricks.com/wp-content/uploads/2014/05/flex-wrap.svg)

###justify-content
Essa propriedade define o alinhamento ao longo do eixo principal. Ajuda a distribuir o espaço extra quando os itens não são flexíveis. Use uma das classes a seguir definir o alinhamento.

* `.start-justified`: (padrão) Os itens são alinhados no começo da linha *(Não é necessario adicionar esta classe)*
* `.center-justified`: Os itens são centralizados ao longo da linha
* `.end-justified`: Os itens ficam alinhados ao final da linha
* `.justified`:Os itens são igualmente distribuídos na linha com o primeiro no inicio da linha e o ultimo no final
* `.around-justified`: Os itens são igualmente distribuídos na linha, com espaços iguais entre eles.

![justify-content](http://css-tricks.com/wp-content/uploads/2013/04/justify-content.svg)

*Note que na classe `.around-justified` visualmente os espaços não são iguais, desde que todos os itens tem espaços iguais em todos os lados, logo os espaços das borda são metade dos espaços entre os itens.*

###align-items

Essa propriedade define como os itens serão alinhados no eixo transversal do seu container. Por padrão os itens se alongam para preencher o container. Use as classes a seguir para definir um alinhamento alternativo.

* `.start`: O itens ficam alinhados no inicio do eixo transversal
* `.center`: Os itens são centralizados no eixo transversal
* `.end`: Os itens ficam alinhados no final do eixo transversal

![align-itens](http://css-tricks.com/wp-content/uploads/2014/05/align-items.svg)

*Para centralizar os itens nos dois eixos, pode se usar a classe `.center-center`*

