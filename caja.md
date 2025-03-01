# Modelo de Caja

### Caja

```css
    span { /*Etiqueta de linea */
      /*Fondo de la caja */
      background: red;
      /*Espacio entre el contenido y la caja */
      padding: 10px; 
      /*Borde de la caja */
      border: 10px solid blue; 
      /*Margen alrededor de la caja */
      margin: 20px; 
      /*Ancho de la caja (content-box) */
      width: 100px; 
      /*Alto de la caja (content-box)*/
      height: 100px;
      box-sizing: border-box; /*Se incluye el margin, border, padding y el contenido se moldea */
      display: block; /* Transforma la etiqueta en una etiqueta de bloque */ 
    }
```
OJO: Es una buena practica usar `box-sizing: border-box`, por default.