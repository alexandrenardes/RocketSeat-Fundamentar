Podemos usar a ferramenta de desenvolvedor do próprio navegador para visualizar as especificações dos elementos da página

image.png

💻 Exemplo:
HTML:

<div>
	CSS é incrível!
</div>
CSS:

div {
   width: 100px; 
   height: 100px;
   border: 1px solid red;
   margin: 10%;
}
Esse é o resultado obtido ao usar o código acima:

image.png

Quando o padding é adicionado (padding: 0 20px;) faz com que aumente a largura da caixa, deixando de respeitar os 100px de largura:

image.png

E é por isso que é tão importante conhecer a propriedade do box-sizing.

Por padrão o navegador vai calcular o tamanho da caixa pelo content-box e vai somar com os outros boxes, no exemplo acima no lugar de 100px a caixa vai ficar com uma largura de 140px. Para que isso não aconteça, é possível mudar qual vai ser a referência para o calculo do tamanho da caixa adicionando a propriedade box-sizing: border-box;.

Dessa forma o elemento vai ficar com a largura (width) determinado, que no caso do exemplo citado é de 100px.

image.png

Normalmente usa-se o código abaixo como forma de "resetar" o box-sizing que vem por padrão nos navegadores.

* {
   box-sizing: border-box;
}
O seletor * seleciona todos os elementos da página.