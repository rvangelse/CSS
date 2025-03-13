# Dinamismo

### Transformaciones
Las `transformaciones` permiten agregarles una mayor interactividad a tus elementos, van de la mano con las ` animaciones`

```css

/* Translaciones */
div {
    width: 100px;
    height: 100px;
    background-color: coral;
    transform: translateX(50px); /* Translacion en el eje X */
    transform: translateY(50px); /* Translacion en el eje Y */
    transform: translate(50px, 50px); /* Translacion en los ejes X e Y */
}

/* Agrandamientos */
div {
    width: 100px;
    height: 100px;
    background-color: skyblue;
    transform: scaleX(1.5); /* Agranda al elemento en su eje X */
    transform: scaleY(1.5); /* Agranda al elemento en su eje Y */
    transform: scale(.5); /* Agranda al elemento en sus ejes X e Y */
}

/* Rotaciones */
div {
    width: 100px;
    height: 100px;
    background-color: lightgreen;
    transform: rotateX(30deg); /* Rota al elemento sobre su eje X */
    transform: rotateY(30deg); /* Rota al elemento sobre su eje Y */
    transform: rotate(30deg); /* Rota al elemento sobre sus ejes X e Y */
}

/* Distorsiones */
div {
    width: 100px;
    height: 100px;
    background-color: plum;
    transform: skewX(30deg); /* Distorsiona al elemento en su eje X */
    transform: skewY(30deg); /* Distorsiona al elemento en su eje Y */
    transform: skew(30deg, 20deg); /* Distorsiona al elemento en sus ejes X e Y */
}

/* Transformaciones completas */
div {
    width: 100px;
    height: 100px;
    background-color: aquamarine;
    transform: translate(50px, 50px) scale(.8) rotate(.3turn) skew(30deg, 20deg);
}
```
OJO: No todos los elementos se pueden transformar.

---
### Transiciones

