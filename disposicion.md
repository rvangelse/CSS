# Disposición

### Diseños

`Layout`es una forma de estructurar diferentes partes de una aplicacion/pagina web de forma que estas ocupen un espacio que sea coherente.

Ejemplo de `Layout`:

<p align="center">
  <img src="imagenes/grafico7.jpg" width="300">
</p>

OJO: Antes se organizaban los elementos de una aplicacion/pagina web usando tablas.

OJO: Es una buena practica, usar `Flexbox` y `CSS Grid` para diseñar tus layouts.

---

### Posiciones

```css
div {
  width: 80px;
  height: 80px;
  position: relative; /* Sus elementos hijos lo usaran como sistema de referencia para su posicion */
}

#primero {
  /* Posicion por default */
  position: static;

  /* Posicion relativa al flujo del documento */
  position: relative;
  top: 10px;
  left: 50px;
  bottom: 20px;
  right: 10px;

  /* Posicion relativa a un sistema de referencia, fuera del flujo del documento */
  position: absolute;
  z-index: 1; /* Variable de altura relativa */
  left: 20px;
  top: 40px;

  /* Igual que absolute, solo que se mantiene flotando */
  position: fixed;
  left: 20px;
  top: 40px;
}
```

OJO: Si no especificas un padre como `relative` al usar `position: absolute` o `position: fixed`, el padre sera el documento html.

---

### Flotados

Son muy utiles cuando quieres envolver una imagen o contenedor con texto, tipo nota-periodico.

```css
div {
  display: inline-block;
  width: 80px;
  height: 80px;
}

#primero { 
  float: left; /* El elemento flota a la izquierda */
}

#segundo {
  float: right;
}

p {
  text-align: justify;
  clear: both; /* Hace que el texto no envuelva a los floats, los ignora */
}
```
OJO: `overflow: hidden;` evita que los elementos floten fuera de su contenedor.

---
### Caja flexible

