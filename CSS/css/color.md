# Cores

Usamos css para alterar cores do nosso documento.

## Tipos

*Backgrouund-color (para caixas)
*color (para textos)
*border-color (para-caixas)
*outros...

## Valores

Podemos definir os valres por 

*palavra-chave (blue, transparent)
*hexadecimal (#990011)
*funções: rgb, rgba, hsl, hsla

```css
element {
    /* Keyword values */
    color: currentcolor;

    /* <named-color> values */
    color: red;
    color: orange;
    color: tan;
    color: rebeccapurple;

    /* <hex-color> values 0-F */
    color: #090; /* RED GREEN BLUE */
    color: #009900;
    color: #090a;
    color: #009900aa;

    /* <rgb()> values */
    color: rgb(34, 12, 64, 0.6); /*00-255*/
    color: rgba(34, 12, 64, 0.6);
    color: rgb(34, 12, 64 / 0.6);
    color: rgba(34, 12, 64 / 0.3);
    color: rgb(34, 12, 64 / 60%);
    color: rgba(34, 12, 64 / 30%);


    /* <hsl()> */
    color: hsl(30, 100%, 50%, 0.6); /* Hue- Saturation - Lumince*/
    color: hsla(30, 100%, 50%, 0.6);
    color: hsl(30 100% 50% /0.6);
    color: hsla(30 100% 50% / 0.6);
    color: hsl(30.0 100% 50% / 60%);
    color: hsla(30.2 100% 50% / 60%);

    /* Global values */
    color: inherit;
    color: initial;
    color: unset;

}
```
##Referência

Podemos definir os valores por

*palavra-chave (blue, transparent)
*hexadecimal (#990011)
*funções: rgb, rgba, hsl, hsla

https://developer.mozilla.org/pt-BR/docs/Web/CSS/color_value








## Background

- Define um fundo para o nosso elemneto
- Sua área de atuação é a caixa toda
- por padrao,, é trasparente

### Exemplos

- Usar cores Sólidas
- Usae imagens
- Controlar
    -a posição das imagens,
    - se elas se repetem ou não
    - o tamanho delas na caixa
- Usar cor e imagem juntas
- Usar cor gradiente

```css
header {
    background-color: rgb(55, 100, 50);
    background-image: url();
    background-repeat: no-repeat;
    background-position: center;
    background-size: contain; 
    background-origin: border-box; /* content-box | padding-box */
    background-clip: border-box; /* content-box | padding-box  */
    background: linear-gradient( 270deg, red, yellow)/* ate mis cores*/ /*radial*/;

    background-attachment: fixed;


    background: ;

}
```


