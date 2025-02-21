# Fundamentos de CSS 

### Sintaxis

<p align="center">
  <img src="imagenes/grafico1.png" width="300">
</p>

OJO: Siempre verifica detenidamente tus selectores y asegúrate de que las propiedades estén correctamente asignadas. Recuerda usar el punto (.) para las clases y numeral (#) para las id.

---
### Selectores

```css
    p { /* Selector de etiquetas */
      color: blue;
      font-size: 25px;
    }

    .clase-texto { /* Selector de clases */
      color: red;
      font-size: 25px;
    }

    #texto-unico { /* Selector de id */
      color: green;
      font-size: 25px;
    }

    .clase-texto span { /* Selector de una etiqueta en una clase */
      color: purple;
      font-size: 25px;
    }

    p,
    span { /* Selector de un grupo de etiquetas */
      text-decoration: underline;
    }
```
El `*` es el selector global.

OJO: Es recomendable siempre agrupar elementos en clases y usar las id, en casos especiales.

OJO: Es una buena practica definir las clases usando `minusculas` y `-`. 





