# Propriedade do Flex Container

* Direção dos itens
* Multi linhas
* Alinhamento
    * principal
    * cruzado
* Espaços entre os itens

```css
.box {
    display: flex;

}
```

# Direção dos itens

- Flex é uma dimensão (horizontal ou vertial)
- Podemos mudar a direção com `flex-direction`
- valores: ( row | row-reverse | column | colmn-reverse )

```css
.container{
    display:flex;
    flex-direction: row-reverse;

}
```
# flex-wrap

- Podemos usar multi linhas.
- Cada nva linha, um novo felx container

```html
<div class="box">
    <div>A</div>
    <div>B</div>
    <div>C</div>
    <div>D</div>
</div>
```
```css
.box{
    /* display: flex; */
    flex-wrap: wrap;
    justify-content: center;

    border: 1px dashed red;
}

.box div {
    border: 1px solid;

    /* width: 80px; */
}
```
# flex-flow

- shorthand
- flex-directon || flex-wrap


# justify-content

- Alinhamento dos elementos dentro do container
- Distribuição dos elementos

## valores

- flex-start
- flex-end
-center
-space-around
-space-between
-space-evenly

# Align-items

- Alinhamento dos elementos no eixo cruzado

## valores

- stretch
- flex-start
- flex-end
- center


# Gap

- Espaços entre os elementos

## valores

- Unidade de medidas
- fixas: px, pt
- flexíveis: %, em, rem.


## Propriedade para os itens

- flex-basis
- flex-grow
- flex-shrink
- flex
- order

# flex-grow

- O crescimento do item dentro do container em relação aos espaços vazios.

# flex-shrink

- O encolher do item dentro do container.

# flex

- shorthand
- flex-grow | flex-shrink | flex- basis
- podem ter 1, 2 ou 3 valores


# Order

- Ordena os items dentro da caixa