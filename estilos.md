# Estilos

### Fondo
```css
html {
    height: 100%; /* Cubre todo la pagina */
}

body { /* El tamaño se adapta a los elementos */
    margin: 0;
    /* Agregar imagen de fondo */
    /* Imagen - Repeticion - Color */
    background: url(http://www.xaviro.com/assets/img/skills/css.svg) no-repeat, blue;
    /* Fondo por parametros */
    background-repeat: no-repeat;
    background-position: center;
    background-size: 100px;
    background-color: blue;
}
```
---
### Color
```css
h1 {
    /* Color del texto */
    color: blue; 
    /* Color del fondo */
    background: gray;
    /* Color del borde */
    border: solid 10px green;
    opacity: 0.5;
    /* Colores en RGB */
    color: rgb(255, 0, 0);
    /* Colores en RGBA */
    color: rgba(255, 0, 0, 1);
    /* Colores en Hexadecimal */
    color: #0011ff;
}
```
OJO: Es recomendable usar los formatos `RGB` y `RGBA` 

OJO: Prueba este [recurso](https://gradients.app/es/new) para crear gradientes.

---
### Modelos

```css
div {
    /* Modelo hsl (Es mas tecnico) */
    /* Matiz - Saturacion - Luz */
    color: hsl(120, 100%, 50%);
    /* Modelo hsla */
    /* Matiz - Saturacion - Luz - Alfa(Transparencia) */
    color: hsla(120, 100%, 50%, 0.5);
    /* Modelo lab (Tiene mas precision) (Uso cientifico) */
    background-color: lab(100 0 100);
    /* Modelo lch (Ayuda mucho con los contrastes) */ 
    /* Luminosidad - Croma - Matiz */
    background-color: lch(40% 100 0);
    /* Modelo oklch (Funciona igual que lch, pero es de uso cientifico) */
    background-color: oklch(0.41 0.44 1.18);
}
```  
OJO: Puedes usar herramientas como [lab](https://observablehq.com/@d3/lab-color-picker) y [lch](https://lch.oklch.com/#70,39,227,100) para tener una mejor visualizacion de los colores en cada modelo. 

---

### Mezcla de colores 

```css

div {   /* Mezcla de colores usando el modelo rgb */
        background-color: color-mix(in srgb, red 50%, blue 50%);
        /* Mezcla de colores usando el modelo hsl */
        background-color: color-mix(in hsl, red 50%, blue 50%);
        /* Mezcla de colores usando el modelo lch */ 
        background-color: color-mix(in lch, red 50%, blue 50%); 
}
```
---
### Colores relativos
Sirve para transformar un color a otro.

```css
:root {
        --principal: blue; /* Declaro una variable global "principal" */
}

div {
      /* Transformacion del color azul usando el modelo hsl */
      background: hsl(from var(--principal) calc(h + 100) s l);
}
```



