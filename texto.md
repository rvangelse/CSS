# Texto en CSS

### Fuentes

```html
<head>
  <!-- Forma 1 para importar fuentes (HTML) -->
  <link rel="preconnect" href="https://fonts.gstatic.com" />
  <link href="https://fonts.googleapis.com/css2?family=Ubuntu+Mono&display=swap" rel="stylesheet" />
  <style>
    /* Forma 2 para importar fuentes (CSS) */
    @import url("https://fonts.googleapis.com/css2?family=Ubuntu+Mono&display=swap");

    p {
      font-family: "Ubuntu Mono", monospace; /* Fuente */
      font-weight: lighter; /* Grosor de la fuente */
      font-style: oblique; /* Estilo de la fuente */
      font-size: 25px; /* Tamaño de la fuente */
    }
  </style>
</head>
```
OJO: Puedes importar fuentes de [Google](https://fonts.google.com/).

---
### Transformaciones
Puedes usar el atributo `text-transform` para transformar un texto de mayusculas a minusculas y viceversa, usando CSS.

```css
p{  /* A mayusculas */
    text-transform: uppercase;
    /* A minusculas */ 
    text-transform: lowercase;
    /* A mayusculas solo las primeras letras de cada palabra */ 
    text-transform: capitalize; 
}
```
---

### Espaciamiento

```css
/* Conserva los espacios y saltos de línea */
.preserve {
    white-space: pre;
}
/* No permite saltos de línea y trunca el texto */
.nowrap {
    white-space: nowrap;
}
/* Permite romper palabras largas */
.word-wrap {
    word-wrap: break-word;
}
```
---
