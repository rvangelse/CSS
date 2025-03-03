# Modelo de Caja

### Caja

```css
    span { /* Etiqueta de linea */
      /* Color del fondo de la caja */
      background-color: red;
      /* Espacio entre el contenido y la caja */
      padding: 10px; 
      /* Borde de la caja */
      border: 10px solid blue; 
      /* Margen alrededor de la caja */
      margin: 20px; 
      /* Ancho de la caja */
      width: 100px; 
      /* Alto de la caja */
      height: 100px;
      box-sizing: border-box; /* Se incluye el margin, el border y el padding a las dimensiones de la caja, el contenido se adapta */
      display: block; /* Transforma la etiqueta en una etiqueta de bloque */ 
    }
```
OJO: `box-sizing: content-box` viene por default.
OJO: Es una buena practica usar `box-sizing: border-box`.
