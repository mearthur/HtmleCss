# Box Model

- Fundamental para fazer layout para a web
- Maior facilidade para aplicar o CSS

## O que é?
Uma caixa retangular.
Essa caixa possui propriedades de uma caixa (2D)

- Tamanho (largura x altura)   width | height
- Conteúdo                     content
- Bordas                       border
- Preencimento inteno          padding
-Espaços fora d caixa          magin

*Cada elemento na sua Página, sserá considerado um caixa.*

## Box-sizing

Como será calculao o tamanho total da caixa?
-content-box | border-box

```css
div {
    box-sizing: border-box;

}
```
# Display: block vs displey: inline

-Como as caixas se comportam em relação ás utras caixas
-Comportamento eterno das caixas

**block**
Ocupa toda a linha, colocando o próximo elemento abaixo desse
Width e Height são respeitados
ex: padding, mrgin, border irão fniconar normalmente.


**inline**
Elemento ao lado do outro
Width e Height não funcionam
Somente valores horizontais de margin, padding e border


exemplo.
block: `<p> <div> <secton>`todos os hedings `<h1> <h2>...`
inline: `<a> <strong> <span> <em>`


## Margin

Espaços entre os elementos

- Margin-top | margin-rigt | margin-bottom | margin-left
-values: `<length>` | `<percentage>` | auto

```css
div {
    /* shorthand */
    margin: 12px 16px 10px 4px;
    margin: 12px 16px 0;
    margin: 8px 16px;
    margin: 8px;

}
```
*Cuidado co margin collapsing (top se ajunta ao bottom)


## Padding

Preenchimento interno da caixa

- padding-top | padding-right | padding-bottom | padding-left
- values: `<length>` | `<percentage>`

```css
div {
   /* shorthand */
    padding: 12px 16px 10px 4px;
    padding: 12px 16px 0;
    padding: 8px 16px;
    padding: 8px;
}
```
**
#Padding poderá causar diferença na largura de um elemnto.

#Border ( e outline )

As bordas da caixa

- value: `<border-style>` | `<border-width>` | `<border-color>`
    -style: solid | dotted | dashed | double | groove | ridge | inset | outset
    -width: `<length>`
    -color: `<color>`

```css
div {
    /* shorthand*/
    border-top: solid 2px; /* top | right | bottom | left */

    /* style */
    border: solid;

    /* width <length> | style */
    border: 2px dotted;

    /* style | color */
    border: outset #f33;

    /* width | style | color */
    border: medium dashed green:
}
```
### e outline? 
 - difere em 4 sentidos:
    - Não modifica o tamanho da caixa, pois não é parte do Box Model
    - Poderá ser diferente de retangular
    - Não permite ajuste individuais
    - Mais usado pelo user agent ara acessibilidade

