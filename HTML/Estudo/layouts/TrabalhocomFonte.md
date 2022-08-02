# Trabalho com Fontes

Tipografia Transmite mensagem

    - Negrito
    - Tamaho
    - Estilo

-------------------------------------------

## Basic Font Properties

* font-family
* font-weight
* font-style
* font-size

-------------------------------------------

## Font Family

* Tipo de fonte em um elemento
* Lista de fontes e ordem de prioridade
* inclui *fallback* font

```css
p {
    font-familly: "Times New Roman", Times, serif;
}
```
    - serif
    - sans

-------------------------------------------
## Font weight
 *peso da fonte

 ```css
 p {
     font-weight: bold;
     font-weight: lighter;
     font-weight: normal;

/* Valores globais */
    font-weight: inherit;
    font-weight: initial;
    font-weight: unset;
 }
 ```
-------------------------------------------
## Font Style
* O Estilo da fonte

```css
span {
    font-style: italic;
    font-style: oblique;

/* Global values */
    font-style: inherit;
    font-style: initial;
    font-style: revert;
    font-style: revert-layer;
    font-style: unset;

}
```


-------------------------------------------
## Font Size
* O tamanho da fonte

```css
p {
    font-size: 18px;
}
```
-------------------------------------------
## Web Fonts
-fontes o sistema x fontes da web
- como usar fontes para web?

* @font-face
* @import
* link


### eferências
https://www.w3.org/TR/css-fonts-3/
https://css-tricks.com/snippets/css/using-font-face/


-------------------------------------------
-------------------------------------------
# Atributos mais estilos às fontes

https://developer.mozilla.org/en-US/docs/Learn/CSS/Styling_text/Fundamentals

Arial       	| Sans-serif	
Courier Novo	| Monospace	
Geórgia	        | Serif	
Times New Roman | Serif	
Trebuchet MS	| Sans-serif
verdana         | Sans-serif


##font-variant

* variações na apresentação fonte

```css
p {
    font-variant: small-caps;
}
```
-------------------------------------------
## font-stretch
* alargamento ou encolhimento da fonte
* aceita palavras-chaves como: expanded, condensed, normal
* aceita porcentagens de 50% a 200%

```css
p {font-stretch: expanded;
}
```
https://developer.mozilla.org/en-US/docs/Web/CSS/font-stretch

-------------------------------------------
## letter-spacing 
* Espaços entre caracteres
* Espaços de cada letras

```css
p {
    letter-spacing: 4px;
}
```
https://developer.mozilla.org/en-US/docs/Web/CSS/letter-spacing


-------------------------------------------

## line-height
* Espaços entre linhas
* Pode ser com unidades ou sem unidades de medida
* Comuns: 1.5 ou 2

```css
p {
    line-height: 1.6;
}
```
https://developer.mozilla.org/en-US/docs/Web/CSS/line-height

-------------------------------------------
## text-transform

* Transformação do text

```css
p {
    text-transform: uppercase; /* capitalize | lowercase | none */
}
```

https://developer.mozilla.org/en-US/docs/Web/CSS/text-transform

-------------------------------------------
## text-decoration

* Aparencia decorativa de um texto
* line: underline | overline| line-through
    * podemos aplicar mais de 1 valor 
* style: wavy | dotted | double | dashed | solid
* color: `<color>` values

```css
p{
    text-decoration: underline; /* shorthand */
}
```
https://developer.mozilla.org/pt-BR/docs/Web/CSS/text-decoration

-------------------------------------------
## text-align
* Alinhamento de um texto
```css
p {
    text-align: center; /* left | right | center | justify */
}
```
https://developer.mozilla.org/pt-BR/docs/Web/CSS/text-align

-------------------------------------------
# text-shadow

* Sombra aplicada a um texto
* Permite múltiplos valores

```css
p {
    text-shadow: 1px 1px 1px red,
        2px 2px 1px green; /* offset-x | offeset-y | blur-radius | color */ 
}
```

https://developer.mozilla.org/pt-BR/docs/Web/CSS/text-shadow

-------------------------------------------
## Shorthand

* font-style, font-variant, font-weight, font,stretch, font-size, ine-height, e font-familly.

```css
p {
    /* -style, -variant, -weight, -stretch, -size, line-height, e -familly. */
    font: italic normal bold normal 3e/1.5 helvetica, Arial, sans-serif;
}
```
`.....................`