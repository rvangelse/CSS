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