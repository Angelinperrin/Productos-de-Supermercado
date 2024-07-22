<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Arsel</title>
    <link rel="stylesheet" href="iniciochidocss.css">
    <link rel="icon" type="image/png" href="logo.png">
</head>
<body>

    <header>
        <div id="mySidenav" class="navbar">
            <div class="dropdown">
                <a href="#" class="dropbtn">Inicio</a>
                <div class="dropdown-content">
                    <a href="alimentos.html">Alimentos</a>
                    <a href="electronica.html">Electrónicos</a>
                    <a href="ropa.html">Ropa</a>
                </div>
            </div>
            <a href="carrito.html">Carrito</a>
            <a href="iniciosesion.html">Inicio de Sesion</a>
        </div>
    </header>
    <div class="logo-container">
        <img src="logoxd2.png" alt="Logo de la empresa">
    </div>


    <script>
            function changeImage(imageId, newImageSrc) {
            // Encuentra la imagen por su id
            var imageElement = document.getElementById(imageId);
            // Cambia la fuente de la imagen
            imageElement.src = newImageSrc;
        }
        function addToCart(productName, price, imageSrc) {
            // Obtiene el carrito del localStorage
            let cart = JSON.parse(localStorage.getItem('cart')) || [];

            // Agrega el producto al carrito
            cart.push({ name: productName, price: price, image: imageSrc });

            // Guarda el carrito actualizado en el localStorage
            localStorage.setItem('cart', JSON.stringify(cart));
        }

        
    </script>

    <footer>
        <p>&copy; 2024 Supermercado ARSEL </p>
    </footer>
    
</body>
</html>
