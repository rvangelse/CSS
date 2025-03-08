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
    /* Modelo hsl */
    color: hsl(120, 100%, 50%);
    /* Modelo hsla */
    color: hsla(120, 100%, 50%, 0.5);
    /* Modelo lab */
    background-color: lab(100 0 100);
    /* Modelo lch */ 
    background-color: lch(40% 100 0);
    /* Modelo oklch */
    background-color: oklch(0.41 0.44 1.18);
  }
```  
OJO: Esto es una correccion.


