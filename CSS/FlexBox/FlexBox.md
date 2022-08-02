# Layouts e evolução

Layout tem a ver com a maneira que os elementos estão distribuidos na tela

## Normal flow

Ou Flow Layout é a maneira que os elementos `block` e `ìnline` ficam na página

```html
<p> Texto block com <strong>inline</strong> dentro </p>
```
## Tables

É a maneira de tabelas onde a tag `table` recebe um display `table` fazendo com que os elementos com que os elementos internos como `td` e `tr`possam ser usados para montar uma tabela.

```html
<table>
    <tr>
        <td> Hora </td>
        <td> 20:00 </td>
    </tr>
    <tr>
        <td> Hora </td>
        <td> 20:37 </td>
    </tr>
</table>
```
## Tabless 
Uso das propriedades `float`, `clear`para que os elementos possam mudar de posição na tela.

```html
<div style="float: left">
    esquerda
</div>

<div style="float: right">
    direita
</div>

<div style="clear: both">
    normal
</div>
```
## Flexbox

A caixa se torna flex, fazedo com que os elementos internos possam recber melhor:
- Alinhamento
- Ordenação
- Tamanhos flexíveis

## Terminologia

-Flex Container
    -Flex item
- Nesting
- Axis
    -main
        -start, end
    -cross
        -start, end
-Flex sizing
    -flexível
    -altera windth/height dos intens para preenchimento dos espaços do flex container

```html
<div class="container">
    <div class="item">1</div>
    <div class="item">2</div>
    <div class="item">3</div>
</div>
```
```css
.container{
    display: flex;
    border: 1px solid red;
    height: 200px;


    flex-direction: column;
    justify-content: flex-end;
}

.item{
    background-color: gray;
    border: 1px solid;
    flex: 1;
}
```


 