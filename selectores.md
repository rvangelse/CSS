# Selectores avanzados

### Pseudoclases
Son un subconjuntos de elementos que cumplen cierta caracteristica. Una vez seleccionados nos dejan modificar propiedades muy especificas

```css

/* Elementos sobre los que pose el cursor */
p:hover {
    color: blue;
}

/* Botones que presione */
button:active {
    color: red;
}

/* Inputs que rellene */
input:focus {
    outline: 2px solid green; /* Cambia el borde del borde de la caja de texto*/
}

/* Enlaces que visite */
a:visited {
    color: purple;
}

/* Primer y ultimo hijo de un elemento */
p:first-child {
    font-weight: bold;
}

p:last-child {
    font-style: italic;
}

/* Hijo indexado de un elemento */
p:nth-child(2) { /* Indexe el segundo hijo de "p" */
    color: orange;
}

/* Elementos a los que no les quiero aplicar un estilo */
 p:not(.excluido) { /* No aplico estilo a los elementos de la clase "excluido" */
    text-decoration: underline;
}

/* Elementos del tipo: par, impar, etc */
p:nth-of-type(odd) { /* Hijos de "p" impares */
    background-color: brown;
}

p:nth-of-type(even) { /* Hijos de "p" pares */
    background-color: brown;
} 

/* Elementos checkeados */
input:checked {
    outline: 2px solid blue;
}

/* Elementos que contienen un determinado sub-elemento */
p:has(span) { /* Hijos de "p" que contienen un "span" */
    color: red;
}
```
---
### Pseudoelementos
Son elementos creados directamente desde CSS 

```css
```

