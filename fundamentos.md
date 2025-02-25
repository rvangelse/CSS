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

---
### Cascada y herencia

Cascada es el efecto en el que el último elemento que tiene el mismo estilo y la misma especificidad gana.

```html
<!-- En este caso, por cascada el ultimo "color" es el que se aplica -->
<!DOCTYPE html>
<html>

<head>
  <style>
    p {
      color: red;
    }
  </style>
  <link rel="stylesheet" href="./styles.css" />
</head>

<body>
  <!-- Estilo efectivo -->
  <p style="color: green;">Texto</p> 
</body>

</html>
```
---
### Especificidad

La especificidad del selector pesa mas que la herencia de la cascada, al aplicar estilos.

```html
<!-- Especificidad -->
<!-- Etiqueta/clase/id > id > clase > Etiqueta Especifica > Etiqueta Global -->

<!DOCTYPE html>
<html>

<head>
  <style>
    p.textos#texto1 { /* > */
      color: blue !important;
    }

    p.textos#texto1 { /* > */
      color: green;
    }

    #texto1 { /* > */
      color: yellow;
    }

    .textos { /* > */
      color: orange;
    }

    p { /* > */
      color: red;
    }

    body { /* > */
      color: purple;
      font-size: 25px;
    }
  </style>
</head>

<body>
  <p id="texto1" class="textos">Texto</p>
</body>

</html>
```

OJO: Manten tu CSS lo más simple posible. Utiliza selectores de clase en lugar de selectores de id o de etiquetas cuando sea posible.

---
### Unidades

```css

    h1 { /* Unidades: */
      background: greenyellow;
      /* px, unidad absoluta */
      width: 300px;
      /* %, unidad relativa al tamaño en px del padre */
      width: 50%; 
      /* em, unidad relativa al font-size en px del padre */
      font-size: 3em; /* 3 veces el tamaño del padre */
      /* rem, unidad relativa al font-size en px de la raiz */
      font-size: 3rem;
    }

```
OJO: No uses unidades en `px` para todos los elementos de diseño. Considera el uso de unidades relativas como `em`, `rem` y `%` para crear diseños más flexibles y accesibles.