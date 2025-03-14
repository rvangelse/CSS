# Complementos

### Prefijos y soporte

```css
h1 {
      -webkit-transition: all 4s ease; /* Prefijo de soporte para Chrome */
      -moz-transition: all 4s ease; /* Prefijo de soporte para Mozilla */
      -ms-transition: all 4s ease; /* Prefijo de soporte para Internet Explorer */
      -o-transition: all 4s ease; /* Prefijo de soporte para Opera */
      transition: all 4s ease; /* Soportes unificados */
    }
```
OJO: Existen recursos para hacer esto más fácil, por ejemplo: 

* [Can I use?](https://caniuse.com/), es una página que te muestra en que navegadores esta disponible una determinada propiedad. 

* [autoprefixer](https://www.npmjs.com/package/autoprefixer), es un plugin que se encarga de chequear todo esto.