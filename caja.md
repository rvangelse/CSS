# Modelo de Caja

### Caja

```css
span {
  /* Etiqueta de linea */
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

---

### Margen y relleno

```css
div,span {
  background-color: red;
  /* Arriba-Derecha-Abajo-Izquierda */
  padding: 100px 20px 30px 80px;
  /* Arriba-DerechaIzquierda-Abajo */
  padding: 100px 40px 30px;
  /* ArribaAbajo-DerechaIzquierda */
  padding: 100px 40px;
  /* ArribaDerechaAbajoIzquierda */
  padding: 10px;
  /* Se puede aislar, tambien */
  padding-top: 10px;
  /* Funciona igual para el margin */
  margin: 1px 20px 40px 5px;
  display: inline-block;
}
```

### Borde

```css
span {
  display: inline-block;
  padding: 20px;
  /* Borde simplificado */
  border: outset 15px red;
  /* Borde por parametros */
  border-style: outset;
  border-width: 15px;
  border-color: red;
  /* Borde por direcciones y parametros */
  border-top-color: blue;
  border-right-color: green;
  border-left-color: yellow;
  border-bottom-color: black;

  border-top-style: dotted;

  border-bottom-width: 5px;
}
```
---

### 
