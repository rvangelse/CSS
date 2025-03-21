# Diseño adaptable

### Consulta de medios
Permite modificar los estilos de una pagina web para pantallas especificas.

```css

div {
      display: inline-block;
      width: 100px;
      height: 100px;
}

/* Modificaciones para pantallas que tienen un width maximo de 500px */
@media only screen and (max-width: 500px) { 
    div {
        width: 40px;
        height: 40px;
    }
}

```
OJO: Intenta diseñar tu sitio web con un enfoque `Mobile First`, es decir, comienza diseñando para dispositivos móviles y luego añade `media queries` para pantallas más grandes. 

---
### Consultas de contenedor
Modifica los estilos de contenedores en distintas pantallas.

```css

div {
    container: contenedor-x / inline-size;
    background-color: blue;
}

span {
    background-color: green;
}

@container contenedor-x (width <=200px) {
    span {
        background-color: red;
    }
}
```
---

### Practica 6: Diseño adaptable en CSS

**Codigo**

```html

<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Peliculas animadas</title>
    <style>
    
        body {
            font-family: Arial, sans-serif;
            background-color: #f5f5f5;
            margin: 0;
            padding: 0;
        }

        header {
            background-color: #333;
            color: #fff;
            text-align: center;
            padding: 20px 0;
        }

        button {
            display: none; /* Oculto el boton (Hare que aparezca solo en dispositivos pequeños */
            cursor: pointer;
            padding: 10px;
            background: #333;
            color: #fff;
            border: 1px solid white;
            margin: auto;
            text-align: center;
        }

        main {
            display: flex;
            justify-content: center;
            margin-top: 100px;
            flex-wrap: wrap;
        }

        div {
            background-color: #fff;
            border: 1px solid #ddd;
            border-radius: 5px;
            padding: 15px;
            margin: 20px;
            width: 300px;
            height: 400px;
            text-align: center;
        }

        div img {
            width: 100%;
            height: 220px;
            margin-bottom: 10px;
        }

        @media (max-width: 600px) {

            main{
                margin-top: 50px;
            }

            button {
                display: block; /* Aparece el boton */
            }
        }
    </style>

</head>
<body>
    <header>
        <h1>Peliculas animadas</h1>
        <button>Menu</button>
    </header>
    <main>
        <div>
            <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTl23zkX9gH_foiNDMrB4wzeZXRSDyt93tcUw&s" alt="Producto 1">
            <h3>El cadaver de la novia</h3>
            <p>Descripcion pelicula 1.</p>
            <p>$19.99</p>
            <a href="#">Comprar</a>
        </div>
        <div>
            <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQslOTo10Q9LJAu_Awi50aNMncjS1_Ii3XBffwn1XqD4AlZKZjQfMUJ2k_TB11m-PpD9CU&usqp=CAU" alt="Producto 2">
            <h3>Moana</h3>
            <p>Descripcion pelicula 2.</p>
            <p>$24.99</p>
            <a href="#">Comprar</a>
        </div>
        <div>
            <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSAEZhGDE9pqpNySzhgESK-sregFuzzFt0MQ5_jkCzfea-heN8SdSG4kNh9Hb9UqOU5t6E&usqp=CAU" alt="Producto 3">
            <h3>Enredados</h3>
            <p>Descripcion pelicula 3.</p>
            <p>$29.99</p>
            <a href="#">Comprar</a>
        </div>
    </main>
</body>
</html>
```
**Output**

<div style="display: flex; justify-content: space-around; flex-wrap: wrap; ">
  <img src="imagenes/grafico9.png" height="320" width="60%" >
  <img src="imagenes/grafico10.png" height="320"  width="25%" >
</div>

