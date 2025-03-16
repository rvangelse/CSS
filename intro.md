# CSS

CSS (Cascading Style Sheets) es un lenguaje de estilo utilizado para describir la apariencia y el formato de un documento escrito en HTML, te permite darle estilo y diseño a tu sitio.

CSS fue propuesto por primera vez por Håkon Wium Lie en 1994. En ese momento, Lie estaba trabajando con Tim Berners-Lee en el CERN. 

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
OJO: En proyectos muy pequeños, pruebas o prototipos usa CSS en la etiqueta `<style>` por simplicidad. En proyectos grandes, usa CSS en archivos externos.

OJO: Es una buena practica resetear los estilos de un proyecto, al iniciarlo.

Puedes usar `resets` como [meyerweb](https://cdnjs.cloudflare.com/ajax/libs/meyer-reset/2.0/reset.min.css).

---
### Recursos 

* [mdn web docs](https://developer.mozilla.org/en-US/docs/Web/CSS) (Página de consultas)

* [W3](https://www.w3.org/Style/CSS/specs.en.html) (Contenido más avanzado)