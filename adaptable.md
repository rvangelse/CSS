# Diseño adaptable

### Consulta de medios
Permite modificar los estilos de una pagina web para pantallas especificas.

```css

div {
      display: inline-block;
      width: 100px;
      height: 100px;
}

/* Modificaciones para pantallas que tienen un width maximo de 500px */
@media only screen and (max-width: 500px) { 
    div {
        width: 40px;
        height: 40px;
    }
}

```
OJO: Intenta diseñar tu sitio web con un enfoque `Mobile First`, es decir, comienza diseñando para dispositivos móviles y luego añade `media queries` para pantallas más grandes. 

---
### Consultas de contenedor
Modifica los estilos de contenedores en distintas pantallas.

```css

div {
    container: contenedor-x / inline-size;
    background-color: blue;
}

span {
    background-color: green;
}

@container contenedor-x (width <=200px) {
    span {
        background-color: red;
    }
}
```
---

### Practica 6: Diseño adaptable en CSS

**Codigo**

```html

