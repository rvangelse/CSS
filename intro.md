# CSS

CSS (Cascading Style Sheets) es un lenguaje de estilo utilizado para describir la apariencia y el formato de un documento escrito en HTML, te permite darle estilo y diseño a tu sitio.

CSS fue propuesto por primera vez por Håkon Wium Lie en 1994. En ese momento, Lie estaba trabajando con Tim Berners-Lee en el CERN. 

```html
<!DOCTYPE html>
<html>

<head>
  <style> <!-- CSS -->
    p /* Selector */ {
      color: red; /* Estilo */
    }
  </style>
</head>

<body>
  <p>Hola Mundo</p>
</body>

</html>
```
OJO: En proyectos muy pequeños, pruebas o prototipos usa CSS en la etiqueta `<style>` por simplicidad. En proyectos grandes, usa CSS en archivos externos.

**Otro ejemplo:**

```css
a {
	color: red;
	text-decoration: none;
}
a:hover{ /* Al posar el mouse sobre el enlace este se torna verde */
    color:green;
}
a:active{ /* Al dar click sobre el enlace este se subraya */
    text-decoration: underline;
}
```
OJO: Es una buena practica al iniciar un nuevo proyecto resetear sus estilos.

OJO: Puedes usar `resets` como [meyerweb](https://cdnjs.cloudflare.com/ajax/libs/meyer-reset/2.0/reset.min.css).
