<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Swete Crust - Prototipo Final</title>
    <style>
        /* Estilos Generales y Colores */
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #FFFACD; /* Amarillo claro */
            color: #333;
        }

        h1, h2 {
            font-family: 'Times New Roman', Times, serif;
            font-style: italic;
        }

        /* Encabezado */
        header {
            background-color: #FFFFFF;
            padding: 20px 0;
            text-align: center;
            border-bottom: 3px solid #FF4500; /* Borde rojo */
        }

        .logo-nombre {
            color: #FF4500;
            font-size: 3em;
            margin: 0;
        }

        .tagline {
            color: #666;
            margin-top: 5px;
            font-style: normal;
        }

        /* Barra de Navegación */
        nav {
            background-color: #FFD700; /* Amarillo dorado */
            padding: 10px 0;
            text-align: center;
            position: sticky; /* Barra pegajosa al hacer scroll */
            top: 0;
            z-index: 100;
        }

        nav a {
            color: #333;
            text-decoration: none;
            padding: 10px 15px;
            margin: 0 5px;
            font-weight: bold;
            display: inline-block; /* Para mejor comportamiento en móviles */
        }

        nav a:hover {
            background-color: #FF4500;
            color: #FFFFFF;
            border-radius: 4px;
        }

        /* Contenido Principal y Secciones */
        .container {
            width: 90%;
            max-width: 1200px;
            margin: 20px auto;
            padding: 20px;
            background-color: #FFFFFF;
            border-radius: 8px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
        }

        .seccion-titulo {
            text-align: center;
            color: #FF4500;
            margin-bottom: 30px;
            font-size: 2em;
            border-bottom: 2px solid #FFD700;
            padding-bottom: 10px;
        }

        /* Galería de Productos */
        .galeria-productos {
            display: flex;
            flex-wrap: wrap;
            justify-content: space-around;
            gap: 20px; /* Espacio entre tarjetas */
        }

        .producto-tarjeta {
            width: 300px;
            border: 1px solid #ddd;
            border-radius: 8px;
            overflow: hidden;
            box-shadow: 0 2px 5px rgba(0, 0, 0, 0.05);
            text-align: center;
            padding-bottom: 15px;
            transition: transform 0.3s, box-shadow 0.3s;
            background-color: #fff;
        }

        .producto-tarjeta:hover {
            transform: translateY(-5px);
            box-shadow: 0 8px 15px rgba(0, 0, 0, 0.15);
        }

        .producto-tarjeta img {
            width: 100%;
            height: 220px; /* Altura fija para uniformidad */
            object-fit: cover; /* Recorta la imagen para llenar el espacio sin deformar */
            display: block;
            border-bottom: 3px solid #FFD700;
        }

        .producto-info {
            padding: 15px;
        }

        .producto-nombre {
            font-size: 1.3em;
            color: #333;
            margin: 10px 0;
            font-weight: bold;
        }

        .producto-descripcion {
            font-size: 0.95em;
            color: #666;
            height: 60px; /* Altura fija para descripciones */
            overflow: hidden;
            margin-bottom: 15px;
            line-height: 1.4;
        }

        .producto-precio {
            font-size: 1.5em;
            color: #008000; /* Verde precio */
            font-weight: bold;
            margin: 15px 0;
        }

        .boton-carrito {
            background-color: #FF4500; /* Rojo vibrante */
            color: white;
            border: none;
            padding: 12px 25px;
            text-align: center;
            text-decoration: none;
            display: inline-block;
            font-size: 16px;
            cursor: pointer;
            border-radius: 50px; /* Botones redondeados */
            transition: background-color 0.3s, transform 0.1s;
            font-weight: bold;
        }

        .boton-carrito:hover {
            background-color: #FF6347;
        }
        
        .boton-carrito:active {
             transform: scale(0.98); /* Pequeño efecto al hacer clic */
        }

        /* Footer */
        footer {
            background-color: #333;
            color: white;
            text-align: center;
            padding: 30px 0;
            margin-top: 40px;
        }
    </style>
</head>
<body>

    <header>
        <h1 class="logo-nombre">
            <span style="font-size: 1.2em;">🍪</span>
            Swete Crust
            <span style="font-size: 1.2em;">❤️</span>
        </h1>
        <p class="tagline">¡El toque dulce y artesanal que estabas esperando!</p>
    </header>

    <nav>
        <a href="#pasteles">🍰 Pasteles</a>
        <a href="#rolls">🌀 Rolls Gourmet</a>
        <a href="#galletas">🍪 Galletas Artesanales</a>
        <a href="#carrito">🛒 Carrito (0)</a>
    </nav>

    <div class="container">

        <section id="pasteles">
            <h2 class="seccion-titulo">Pasteles Enteros (Para compartir)</h2>
            <div class="galeria-productos">

                <div class="producto-tarjeta">
                    <img src="https://images.unsplash.com/photo-1578985545062-69928b1d9587?ixlib=rb-4.0.3&auto=format&fit=crop&w=500&q=60" alt="Pastel de Chocolate Intenso">
                    <div class="producto-info">
                        <p class="producto-nombre">Pastel "Muerte por Chocolate"</p>
                        <p class="producto-descripcion">
                            Tres capas de bizcocho húmedo de cacao, relleno y cubierto con ganache de chocolate semi-amargo belga.
                        </p>
                        <p class="producto-precio">$550.00 MXN</p>
                        <button class="boton-carrito">Agregar al Carrito</button>
                    </div>
                </div>

                <div class="producto-tarjeta">
                    <img src="https://images.unsplash.com/photo-1464349095431-e9a21285b5f3?ixlib=rb-4.0.3&auto=format&fit=crop&w=500&q=60" alt="Pastel de Fresa y Nata">
                    <div class="producto-info">
                        <p class="producto-nombre">Pastel Fresas con Crema</p>
                        <p class="producto-descripcion">
                            Clásico y ligero. Bizcocho de vainilla, crema batida natural y abundantes fresas frescas del huerto.
                        </p>
                        <p class="producto-precio">$480.00 MXN</p>
                        <button class="boton-carrito">Agregar al Carrito</button>
                    </div>
                </div>

                <div class="producto-tarjeta">
                    <img src="https://images.unsplash.com/photo-1519869325930-281384150729?ixlib=rb-4.0.3&auto=format&fit=crop&w=500&q=60" alt="Pastel de Vainilla Elegante">
                    <div class="producto-info">
                        <p class="producto-nombre">Pastel Vainilla Imperial</p>
                        <p class="producto-descripcion">
                            Elegancia pura. Bizcocho con auténtica vainilla de Papantla y betún de mantequilla sedoso.
                        </p>
                        <p class="producto-precio">$390.00 MXN</p>
                        <button class="boton-carrito">Agregar al Carrito</button>
                    </div>
                </div>

            </div>
        </section>

        <hr style="border: 0; height: 1px; background: #FFD700; margin: 40px 0;">

        <section id="rolls">
            <h2 class="seccion-titulo">Rolls Gourmet (Pieza Individual)</h2>
            <div class="galeria-productos">

                <div class="producto-tarjeta">
                    <img src="https://images.unsplash.com/photo-1509365465985-25d11c17e812?ixlib=rb-4.0.3&auto=format&fit=crop&w=500&q=60" alt="Roll de Canela Clásico">
                    <div class="producto-info">
                        <p class="producto-nombre">Cinnamon Roll Clásico</p>
                        <p class="producto-descripcion">
                            Masa brioche ultra suave, abundante canela importada y nuestro glaseado especial de queso crema tibio.
                        </p>
                        <p class="producto-precio">$65.00 MXN c/u</p>
                        <button class="boton-carrito">Agregar al Carrito</button>
                    </div>
                </div>

                <div class="producto-tarjeta">
                    <img src="https://images.unsplash.com/photo-1495147466023-ac5c588e2e94?ixlib=rb-4.0.3&auto=format&fit=crop&w=500&q=60" alt="Roll Frutos Rojos">
                    <div class="producto-info">
                        <p class="producto-nombre">Roll de Frutos del Bosque</p>
                        <p class="producto-descripcion">
                            Una explosión frutal. Relleno de compota casera de zarzamoras y frambuesas, con un toque de limón.
                        </p>
                        <p class="producto-precio">$75.00 MXN c/u</p>
                        <button class="boton-carrito">Agregar al Carrito</button>
                    </div>
                </div>
            </div>
        </section>

        <hr style="border: 0; height: 1px; background: #FFD700; margin: 40px 0;">

        <section id="galletas">
            <h2 class="seccion-titulo">Galletas Artesanales (Tamaño Grande)</h2>
            <div class="galeria-productos">

                <div class="producto-tarjeta">
                    <img src="https://images.unsplash.com/photo-1499636138143-963773336891?ixlib=rb-4.0.3&auto=format&fit=crop&w=500&q=60" alt="Galleta Chispas Chocolate">
                    <div class="producto-info">
                        <p class="producto-nombre">La "Chunky" de Chocolate</p>
                        <p class="producto-descripcion">
                            Galleta gruesa y suave por dentro, cargada con trozos gigantes de chocolate semi-amargo derretido.
                        </p>
                        <p class="producto-precio">$55.00 MXN c/u</p>
                        <button class="boton-carrito">Agregar al Carrito</button>
                    </div>
                </div>

                <div class="producto-tarjeta">
                    <img src="https://images.unsplash.com/photo-1618923850107-d1a234d7a73a?ixlib=rb-4.0.3&auto=format&fit=crop&w=500&q=60" alt="Galleta Avena Saludable">
                    <div class="producto-info">
                        <p class="producto-nombre">Galleta Avena Suprema (Saludable)</p>
                        <p class="producto-descripcion">
                            Opción nutritiva. Avena integral, pasas, nueces, endulzada con miel de abeja y un toque de canela.
                        </p>
                        <p class="producto-precio">$60.00 MXN c/u</p>
                        <button class="boton-carrito">Agregar al Carrito</button>
                    </div>
                </div>

                <div class="producto-tarjeta">
                    <img src="https://images.unsplash.com/photo-1621236378699-8597fafedbd4?ixlib=rb-4.0.3&auto=format&fit=crop&w=500&q=60" alt="Galleta Rellena de Nutella">
                    <div class="producto-info">
                        <p class="producto-nombre">Bomba Rellena de Avellana</p>
                        <p class="producto-descripcion">
                            Nuestra galleta de mantequilla dorada por fuera, con un corazón líquido y abundante de crema de avellanas.
                        </p>
                        <p class="producto-precio">$65.00 MXN c/u</p>
                        <button class="boton-carrito">Agregar al Carrito</button>
                    </div>
                </div>
            </div>
        </section>

    </div>

    <footer>
        <p>&copy; 2024 Swete Crust S.A. de C.V. | Prototipo de Aplicación Web</p>
        <p>Calidad Artesanal Mexicana | Aviso de Privacidad | Términos y Condiciones</p>
    </footer>

</body>
</html>
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Swete Crust - Menú Extendido</title>
    <style>
        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #FFFACD; 
            color: #333;
        }

        header {
            background-color: #FFFFFF;
            padding: 30px 0;
            text-align: center;
            border-bottom: 5px solid #FF4500;
        }

        .logo-nombre {
            color: #FF4500;
            font-size: 3.5em;
            margin: 0;
            font-family: 'Times New Roman', serif;
            font-style: italic;
        }

        nav {
            background-color: #FFD700;
            padding: 15px 0;
            text-align: center;
            position: sticky;
            top: 0;
            z-index: 1000;
            box-shadow: 0 4px 10px rgba(0,0,0,0.1);
        }

        nav a {
            color: #333;
            text-decoration: none;
            padding: 10px 15px;
            margin: 0 5px;
            font-weight: bold;
            border-radius: 20px;
            transition: 0.3s;
        }

        nav a:hover {
            background-color: #FF4500;
            color: white;
        }

        .container {
            width: 95%;
            max-width: 1300px;
            margin: 30px auto;
            background-color: #FFFFFF;
            padding: 20px;
            border-radius: 20px;
        }

        .seccion-titulo {
            text-align: center;
            color: #FF4500;
            font-size: 2.5em;
            margin: 50px 0 30px 0;
            border-bottom: 3px solid #FFD700;
            display: inline-block;
            width: 100%;
        }

        /* Rejilla de productos optimizada para muchos elementos */
        .galeria-productos {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(280px, 1fr));
            gap: 25px;
        }

        .producto-tarjeta {
            border: 1px solid #eee;
            border-radius: 15px;
            overflow: hidden;
            transition: 0.3s;
            background: #fff;
            display: flex;
            flex-direction: column;
            box-shadow: 0 4px 6px rgba(0,0,0,0.05);
        }

        .producto-tarjeta:hover {
            transform: translateY(-8px);
            box-shadow: 0 12px 20px rgba(0,0,0,0.1);
        }

        .producto-tarjeta img {
            width: 100%;
            height: 200px;
            object-fit: cover;
        }

        .producto-info {
            padding: 15px;
            text-align: center;
            flex-grow: 1;
        }

        .producto-nombre {
            font-size: 1.2em;
            font-weight: bold;
            color: #222;
            margin: 10px 0;
        }

        .producto-precio {
            font-size: 1.4em;
            color: #2e7d32;
            font-weight: bold;
            margin: 10px 0;
        }

        .boton-carrito {
            background-color: #FF4500;
            color: white;
            border: none;
            padding: 12px;
            border-radius: 25px;
            font-weight: bold;
            cursor: pointer;
            width: 100%;
            transition: 0.3s;
        }

        .boton-carrito:hover {
            background-color: #e03e00;
        }

        footer {
            background-color: #222;
            color: white;
            text-align: center;
            padding: 40px 0;
            margin-top: 50px;
        }
    </style>
</head>
<body>

    <header>
        <h1 class="logo-nombre">🍪 Swete Crust ❤️</h1>
        <p>¡Explora nuestro catálogo extendido con más de 25 delicias!</p>
    </header>

    <nav>
        <a href="#galletas">🍪 Galletas (20+)</a>
        <a href="#bebidas">☕ Bebidas</a>
        <a href="#pasteles">🍰 Pasteles</a>
        <a href="#rolls">🌀 Rolls</a>
    </nav>

    <div class="container">

        <section id="bebidas">
            <h2 class="seccion-titulo">☕ Bebidas Especiales</h2>
            <div class="galeria-productos">
                <div class="producto-tarjeta">
                    <img src="https://images.unsplash.com/photo-1541167760496-162955ed8a9f?w=400" alt="Cafe Latte">
                    <div class="producto-info">
                        <p class="producto-nombre">Latte Vainilla Madagascar</p>
                        <p class="producto-precio">$75.00 MXN</p>
                        <button class="boton-carrito">Agregar</button>
                    </div>
                </div>
                <div class="producto-tarjeta">
                    <img src="https://images.unsplash.com/photo-1572286258217-40142c1c6a70?w=400" alt="Chocolate Caliente">
                    <div class="producto-info">
                        <p class="producto-nombre">Chocolate Abuelita Gourmet</p>
                        <p class="producto-precio">$65.00 MXN</p>
                        <button class="boton-carrito">Agregar</button>
                    </div>
                </div>
                <div class="producto-tarjeta">
                    <img src="https://images.unsplash.com/photo-1517701604599-bb28b3e50822?w=400" alt="Frappe">
                    <div class="producto-info">
                        <p class="producto-nombre">Frappé Cookies & Cream</p>
                        <p class="producto-precio">$95.00 MXN</p>
                        <button class="boton-carrito">Agregar</button>
                    </div>
                </div>
                <div class="producto-tarjeta">
                    <img src="https://images.unsplash.com/photo-1556679343-c7306c1976bc?w=400" alt="Smoothie">
                    <div class="producto-info">
                        <p class="producto-nombre">Smoothie de Frutos Rojos</p>
                        <p class="producto-precio">$85.00 MXN</p>
                        <button class="boton-carrito">Agregar</button>
                    </div>
                </div>
            </div>
        </section>

        <section id="galletas">
            <h2 class="seccion-titulo">🍪 El Paraíso de las Galletas</h2>
            <div class="galeria-productos">
                
                <div class="producto-tarjeta">
                    <img src="https://images.unsplash.com/photo-1499636138143-963773336891?w=400" alt="Galleta 1">
                    <div class="producto-info">
                        <p class="producto-nombre">Classic Choco-Chip</p>
                        <p class="producto-precio">$50.00 MXN</p>
                        <button class="boton-carrito">Agregar</button>
                    </div>
                </div>
                <div class="producto-tarjeta">
                    <img src="https://images.unsplash.com/photo-1618923850107-d1a234d7a73a?w=400" alt="Galleta 2">
                    <div class="producto-info">
                        <p class="producto-nombre">Avena y Arándanos</p>
                        <p class="producto-precio">$55.00 MXN</p>
                        <button class="boton-carrito">Agregar</button>
                    </div>
                </div>
                <div class="producto-tarjeta">
                    <img src="https://images.unsplash.com/photo-1621236378699-8597fafedbd4?w=400" alt="Galleta 3">
                    <div class="producto-info">
                        <p class="producto-nombre">Red Velvet Rellena</p>
                        <p class="producto-precio">$65.00 MXN</p>
                        <button class="boton-carrito">Agregar</button>
                    </div>
                </div>
                <div class="producto-tarjeta">
                    <img src="https://images.unsplash.com/photo-1558961363-fa8fdf82db35?w=400" alt="Galleta 4">
                    <div class="producto-info">
                        <p class="producto-nombre">Doble Chocolate Belga</p>
                        <p class="producto-precio">$60.00 MXN</p>
                        <button class="boton-carrito">Agregar</button>
                    </div>
                </div>
                <div class="producto-tarjeta">
                    <img src="https://images.unsplash.com/photo-1590080875515-8a3a8dc5735e?w=400" alt="Galleta 5">
                    <div class="producto-info">
                        <p class="producto-nombre">Matcha & White Choco</p>
                        <p class="producto-precio">$65.00 MXN</p>
                        <button class="boton-carrito">Agregar</button>
                    </div>
                </div>
                <div class="producto-tarjeta">
                    <img src="https://images.unsplash.com/photo-1557089706-68d02dbda277?w=400" alt="Galleta 6">
                    <div class="producto-info">
                        <p class="producto-nombre">Kinder Bueno Cookie</p>
                        <p class="producto-precio">$75.00 MXN</p>
                        <button class="boton-carrito">Agregar</button>
                    </div>
                </div>
                <div class="producto-tarjeta">
                    <img src="https://images.unsplash.com/photo-1559622214-f8a9850965bb?w=400" alt="Galleta 7">
                    <div class="producto-info">
                        <p class="producto-nombre">Limón y Semillas de Amapola</p>
                        <p class="producto-precio">$50.00 MXN</p>
                        <button class="boton-carrito">Agregar</button>
                    </div>
                </div>
                <div class="producto-tarjeta">
                    <img src="https://images.unsplash.com/photo-1600431521340-491eca880813?w=400" alt="Galleta 8">
                    <div class="producto-info">
                        <p class="producto-nombre">Nutella Explosion</p>
                        <p class="producto-precio">$70.00 MXN</p>
                        <button class="boton-carrito">Agregar</button>
                    </div>
                </div>
                <div class="producto-tarjeta">
                    <img src="https://images.unsplash.com/photo-1597481499750-3e6b22637e12?w=400" alt="Galleta 9">
                    <div class="producto-info">
                        <p class="producto-nombre">Oreo Cheesecake Cookie</p>
                        <p class="producto-precio">$65.00 MXN</p>
                        <button class="boton-carrito">Agregar</button>
                    </div>
                </div>
                <div class="producto-tarjeta">
                    <img src="https://images.unsplash.com/photo-1584001300632-3ed1327a67d6?w=400" alt="Galleta 10">
                    <div class="producto-info">
                        <p class="producto-nombre">Caramelo Salado y Nuez</p>
                        <p class="producto-precio">$60.00 MXN</p>
                        <button class="boton-carrito">Agregar</button>
                    </div>
                </div>
                <div class="producto-tarjeta"><img src="https://images.unsplash.com/photo-1558961363-62f7cc1c6761?w=400"><div class="producto-info"><p class="producto-nombre">Mantequilla Real</p><p class="producto-precio">$50.00 MXN</p><button class="boton-carrito">Agregar</button></div></div>
                <div class="producto-tarjeta"><img src="https://images.unsplash.com/photo-1551462147-37885acc3c41?w=400"><div class="producto-info"><p class="producto-nombre">S'mores & Bombón</p><p class="producto-precio">$75.00 MXN</p><button class="boton-carrito">Agregar</button></div></div>
                <div class="producto-tarjeta"><img src="https://images.unsplash.com/photo-1627038162125-866468097f22?w=400"><div class="producto-info"><p class="producto-nombre">Pistacho Supremo</p><p class="producto-precio">$85.00 MXN</p><button class="boton-carrito">Agregar</button></div></div>
                <div class="producto-tarjeta"><img src="https://images.unsplash.com/photo-1551024506-0bccd828d307?w=400"><div class="producto-info"><p class="producto-nombre">Donut Cookie Mix</p><p class="producto-precio">$60.00 MXN</p><button class="boton-carrito">Agregar</button></div></div>
                <div class="producto-tarjeta"><img src="https://images.unsplash.com/photo-1544070078-a212eda27b49?w=400"><div class="producto-info"><p class="producto-nombre">Pumpkin Spice (Temp)</p><p class="producto-precio">$65.00 MXN</p><button class="boton-carrito">Agregar</button></div></div>
                <div class="producto-tarjeta"><img src="https://images.unsplash.com/photo-1601004890684-d8cbf643f5f2?w=400"><div class="producto-info"><p class="producto-nombre">Fresas con Crema</p><p class="producto-precio">$70.00 MXN</p><button class="boton-carrito">Agregar</button></div></div>
                <div class="producto-tarjeta"><img src="https://images.unsplash.com/photo-1587132137056-bfbf0166836e?w=400"><div class="producto-info"><p class="producto-nombre">Plátano y Cacahuate</p><p class="producto-precio">$55.00 MXN</p><button class="boton-carrito">Agregar</button></div></div>
                <div class="producto-tarjeta"><img src="https://images.unsplash.com/photo-1512411516723-57579893d7c7?w=400"><div class="producto-info"><p class="producto-nombre">Menta & Chocolate</p><p class="producto-precio">$60.00 MXN</p><button class="boton-carrito">Agregar</button></div></div>
                <div class="producto-tarjeta"><img src="https://images.unsplash.com/photo-1534073828943-f801091bb276?w=400"><div class="producto-info"><p class="producto-nombre">Cajeta Rellena</p><p class="producto-precio">$65.00 MXN</p><button class="boton-carrito">Agregar</button></div></div>
                <div class="producto-tarjeta"><img src="https://images.unsplash.com/photo-1558961363-fa8fdf82db35?w=400"><div class="producto-info"><p class="producto-nombre">Crunchy Almond</p><p class="producto-precio">$55.00 MXN</p><button class="boton-carrito">Agregar</button></div></div>

            </div>
        </section>

    </div>

    <footer>
        <p>&copy; 2026 Swete Crust S.A. de C.V.</p>
        <p>Precios sujetos a cambio. Calidad 100% Artesanal.</p>
    </footer>

</body>
</html>
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Swete Crust - Catálogo Completo</title>
    <style>
        body {
            font-family: 'Segoe UI', Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #FFFACD;
            color: #333;
        }

        header {
            background-color: #fff;
            text-align: center;
            padding: 30px;
            border-bottom: 5px solid #FF4500;
        }

        .logo-nombre {
            color: #FF4500;
            font-size: 3em;
            margin: 0;
            font-family: 'Times New Roman', serif;
        }

        nav {
            background-color: #FFD700;
            padding: 15px;
            text-align: center;
            position: sticky;
            top: 0;
            z-index: 1000;
        }

        nav a {
            text-decoration: none;
            color: #333;
            font-weight: bold;
            margin: 0 15px;
            padding: 8px 15px;
            border-radius: 20px;
            transition: 0.3s;
        }

        nav a:hover {
            background: #FF4500;
            color: #fff;
        }

        .container {
            max-width: 1200px;
            margin: 20px auto;
            background: #fff;
            padding: 20px;
            border-radius: 15px;
        }

        .seccion-titulo {
            text-align: center;
            color: #FF4500;
            font-size: 2em;
            margin: 40px 0 20px;
            border-bottom: 2px solid #FFD700;
        }

        .grid-productos {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(250px, 1fr));
            gap: 20px;
        }

        .tarjeta {
            border: 1px solid #eee;
            border-radius: 12px;
            overflow: hidden;
            text-align: center;
            padding-bottom: 15px;
            box-shadow: 0 4px 8px rgba(0,0,0,0.1);
        }

        .tarjeta img {
            width: 100%;
            height: 180px;
            object-fit: cover;
            border-bottom: 3px solid #FFD700;
        }

        .precio {
            font-size: 1.3em;
            color: #2e7d32;
            font-weight: bold;
            margin: 10px 0;
        }

        .boton {
            background: #FF4500;
            color: white;
            border: none;
            padding: 10px 20px;
            border-radius: 25px;
            cursor: pointer;
            font-weight: bold;
        }

        footer {
            background: #333;
            color: white;
            text-align: center;
            padding: 20px;
            margin-top: 50px;
        }
    </style>
</head>
<body>

<header>
    <h1 class="logo-nombre">🍪 Swete Crust ❤️</h1>
    <p>Calidad Artesanal Mexicana</p>
</header>

<nav>
    <a href="#bebidas">☕ Bebidas</a>
    <a href="#galletas">🍪 Galletas (20+)</a>
    <a href="#pasteles">🍰 Pasteles</a>
</nav>

<div class="container">

    <section id="bebidas">
        <h2 class="seccion-titulo">☕ Bebidas Calientes y Frías</h2>
        <div class="grid-productos">
            <div class="tarjeta">
                <img src="https://images.unsplash.com/photo-1541167760496-162955ed8a9f?q=80&w=500&auto=format&fit=crop" alt="Latte">
                <h3>Latte Vainilla</h3>
                <p class="precio">$75.00</p>
                <button class="boton">Agregar</button>
            </div>
            <div class="tarjeta">
                <img src="https://images.unsplash.com/photo-1544787210-2213d84ad960?q=80&w=500&auto=format&fit=crop" alt="Chocolate">
                <h3>Chocolate Caliente</h3>
                <p class="precio">$65.00</p>
                <button class="boton">Agregar</button>
            </div>
            <div class="tarjeta">
                <img src="https://images.unsplash.com/photo-1461023058943-07fcbe16d735?q=80&w=500&auto=format&fit=crop" alt="Frappe">
                <h3>Frappé Mocha</h3>
                <p class="precio">$95.00</p>
                <button class="boton">Agregar</button>
            </div>
            <div class="tarjeta">
                <img src="https://images.unsplash.com/photo-1556679343-c7306c1976bc?q=80&w=500&auto=format&fit=crop" alt="Smoothie">
                <h3>Smoothie Fresa</h3>
                <p class="precio">$80.00</p>
                <button class="boton">Agregar</button>
            </div>
        </div>
    </section>

    <section id="galletas">
        <h2 class="seccion-titulo">🍪 Nuestro Gran Galletón (20 Variedades)</h2>
        <div class="grid-productos">
            <div class="tarjeta">
                <img src="https://images.unsplash.com/photo-1499636138143-963773336891?q=80&w=500&auto=format&fit=crop" alt="Cookie">
                <h3>Chispas Clásica</h3>
                <p class="precio">$50.00</p>
                <button class="boton">Agregar</button>
            </div>
            <div class="tarjeta">
                <img src="https://images.unsplash.com/photo-1618923850107-d1a234d7a73a?q=80&w=500&auto=format&fit=crop" alt="Cookie">
                <h3>Avena y Miel</h3>
                <p class="precio">$55.00</p>
                <button class="boton">Agregar</button>
            </div>
            <div class="tarjeta">
                <img src="https://images.unsplash.com/photo-1621236378699-8597fafedbd4?q=80&w=500&auto=format&fit=crop" alt="Cookie">
                <h3>Red Velvet</h3>
                <p class="precio">$65.00</p>
                <button class="boton">Agregar</button>
            </div>
            <div class="tarjeta">
                <img src="https://images.unsplash.com/photo-1558961363-fa8fdf82db35?q=80&w=500&auto=format&fit=crop" alt="Cookie">
                <h3>Doble Chocolate</h3>
                <p class="precio">$60.00</p>
                <button class="boton">Agregar</button>
            </div>
            <div class="tarjeta">
                <img src="https://images.unsplash.com/photo-1590080875515-8a3a8dc5735e?q=80&w=500&auto=format&fit=crop" alt="Cookie">
                <h3>Matcha Special</h3>
                <p class="precio">$70.00</p>
                <button class="boton">Agregar</button>
            </div>
            <div class="tarjeta"><img src="https://images.unsplash.com/photo-1557089706-68d02dbda277?q=80&w=500&auto=format&fit=crop"><h3>Kinder Cookie</h3><p class="precio">$75.00</p><button class="boton">Agregar</button></div>
            <div class="tarjeta"><img src="https://images.unsplash.com/photo-1559622214-f8a9850965bb?q=80&w=500&auto=format&fit=crop"><h3>Limón Glaseado</h3><p class="precio">$50.00</p><button class="boton">Agregar</button></div>
            <div class="tarjeta"><img src="https://images.unsplash.com/photo-1600431521340-491eca880813?q=80&w=500&auto=format&fit=crop"><h3>Nutella Bomb</h3><p class="precio">$70.00</p><button class="boton">Agregar</button></div>
            <div class="tarjeta"><img src="https://images.unsplash.com/photo-1597481499750-3e6b22637e12?q=80&w=500&auto=format&fit=crop"><h3>Oreo Deluxe</h3><p class="precio">$65.00</p><button class="boton">Agregar</button></div>
            <div class="tarjeta"><img src="https://images.unsplash.com/photo-1584001300632-3ed1327a67d6?q=80&w=500&auto=format&fit=crop"><h3>Caramelo Salado</h3><p class="precio">$60.00</p><button class="boton">Agregar</button></div>
            <div class="tarjeta"><img src="https://images.unsplash.com/photo-1558961363-62f7cc1c6761?q=80&w=500&auto=format&fit=crop"><h3>Mantequilla Pura</h3><p class="precio">$50.00</p><button class="boton">Agregar</button></div>
            <div class="tarjeta"><img src="https://images.unsplash.com/photo-1551462147-37885acc3c41?q=80&w=500&auto=format&fit=crop"><h3>S'mores Malvavisco</h3><p class="precio">$75.00</p><button class="boton">Agregar</button></div>
            <div class="tarjeta"><img src="https://images.unsplash.com/photo-1627038162125-866468097f22?q=80&w=500&auto=format&fit=crop"><h3>Pistacho Crunch</h3><p class="precio">$85.00</p><button class="boton">Agregar</button></div>
            <div class="tarjeta"><img src="https://images.unsplash.com/photo-1551024506-0bccd828d307?q=80&w=500&auto=format&fit=crop"><h3>Confeti Party</h3><p class="precio">$55.00</p><button class="boton">Agregar</button></div>
            <div class="tarjeta"><img src="https://images.unsplash.com/photo-1544070078-a212eda27b49?q=80&w=500&auto=format&fit=crop"><h3>Nuez de Macadamia</h3><p class="precio">$80.00</p><button class="boton">Agregar</button></div>
            <div class="tarjeta"><img src="https://images.unsplash.com/photo-1601004890684-d8cbf643f5f2?q=80&w=500&auto=format&fit=crop"><h3>Fresa Rellena</h3><p class="precio">$70.00</p><button class="boton">Agregar</button></div>
            <div class="tarjeta"><img src="https://images.unsplash.com/photo-1587132137056-bfbf0166836e?q=80&w=500&auto=format&fit=crop"><h3>Banana & Choco</h3><p class="precio">$55.00</p><button class="boton">Agregar</button></div>
            <div class="tarjeta"><img src="https://images.unsplash.com/photo-1512411516723-57579893d7c7?q=80&w=500&auto=format&fit=crop"><h3>Menta Choc</h3><p class="precio">$65.00</p><button class="boton">Agregar</button></div>
            <div class="tarjeta"><img src="https://images.unsplash.com/photo-1534073828943-f801091bb276?q=80&w=500&auto=format&fit=crop"><h3>Dulce de Leche</h3><p class="precio">$70.00</p><button class="boton">Agregar</button></div>
            <div class="tarjeta"><img src="https://images.unsplash.com/photo-1459789034005-ba29c5783491?q=80&w=500&auto=format&fit=crop"><h3>Arándano Blanco</h3><p class="precio">$60.00</p><button class="boton">Agregar</button></div>
        </div>
    </section>

</div>

<footer>
    <p>&copy; 2026 Swete Crust S.A. de C.V.</p>
    <p>Si las imágenes no cargan, asegúrate de estar conectado a Internet.</p>
</footer>

</body>
</html>
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Swete Crust - Catálogo Completo y Ubicación</title>
    <style>
        /* Estilos Globales */
        body {
            font-family: 'Segoe UI', Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #FFFACD; /* Amarillo claro */
            color: #333;
            scroll-behavior: smooth;
        }

        header {
            background-color: #fff;
            text-align: center;
            padding: 40px 20px;
            border-bottom: 5px solid #FF4500;
        }

        .logo-nombre {
            color: #FF4500;
            font-size: 3.5em;
            margin: 0;
            font-family: 'Times New Roman', serif;
            font-style: italic;
        }

        nav {
            background-color: #FFD700; /* Dorado */
            padding: 15px;
            text-align: center;
            position: sticky;
            top: 0;
            z-index: 1000;
            box-shadow: 0 2px 5px rgba(0,0,0,0.1);
        }

        nav a {
            text-decoration: none;
            color: #333;
            font-weight: bold;
            margin: 0 10px;
            padding: 8px 15px;
            border-radius: 20px;
            transition: 0.3s;
        }

        nav a:hover {
            background: #FF4500;
            color: #fff;
        }

        .container {
            max-width: 1200px;
            margin: 20px auto;
            background: #fff;
            padding: 30px;
            border-radius: 15px;
            box-shadow: 0 5px 15px rgba(0,0,0,0.05);
        }

        .seccion-titulo {
            text-align: center;
            color: #FF4500;
            font-size: 2.2em;
            margin: 40px 0 25px;
            border-bottom: 3px solid #FFD700;
            padding-bottom: 10px;
        }

        /* Grid de Productos */
        .grid-productos {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(280px, 1fr));
            gap: 25px;
        }

        .tarjeta {
            border: 1px solid #eee;
            border-radius: 15px;
            overflow: hidden;
            text-align: center;
            padding-bottom: 20px;
            transition: transform 0.3s;
            background: #fff;
            box-shadow: 0 4px 8px rgba(0,0,0,0.1);
        }

        .tarjeta:hover {
            transform: translateY(-10px);
        }

        .tarjeta img {
            width: 100%;
            height: 200px;
            object-fit: cover;
            border-bottom: 4px solid #FFD700;
        }

        .precio {
            font-size: 1.4em;
            color: #2e7d32;
            font-weight: bold;
            margin: 10px 0;
        }

        .boton {
            background: #FF4500;
            color: white;
            border: none;
            padding: 12px 25px;
            border-radius: 30px;
            cursor: pointer;
            font-weight: bold;
            transition: 0.3s;
        }

        .boton:hover {
            background: #e63e00;
        }

        /* Sección Ubicación */
        .ubicacion-contenedor {
            display: flex;
            flex-wrap: wrap;
            gap: 20px;
            margin-top: 20px;
        }

        .info-direccion {
            flex: 1;
            min-width: 300px;
            padding: 20px;
            background: #fdfdfd;
            border-left: 5px solid #FF4500;
            border-radius: 8px;
        }

        .mapa-frame {
            flex: 1;
            min-width: 300px;
            height: 400px;
            border-radius: 15px;
            overflow: hidden;
            box-shadow: 0 4px 10px rgba(0,0,0,0.2);
        }

        iframe {
            width: 100%;
            height: 100%;
            border: 0;
        }

        footer {
            background: #333;
            color: white;
            text-align: center;
            padding: 40px 20px;
            margin-top: 50px;
        }
    </style>
</head>
<body>

<header>
    <h1 class="logo-nombre">🍪 Swete Crust ❤️</h1>
    <p>Pastelería Artesanal • El sabor que te enamora</p>
</header>

<nav>
    <a href="#pasteles">🍰 Pasteles</a>
    <a href="#rolls">🌀 Rolls</a>
    <a href="#galletas">🍪 Galletas</a>
    <a href="#bebidas">☕ Bebidas</a>
    <a href="#visitanos">📍 Ubicación</a>
</nav>

<div class="container">

    <section id="pasteles">
        <h2 class="seccion-titulo">🍰 Nuestros Pasteles</h2>
        <div class="grid-productos">
            <div class="tarjeta">
                <img src="https://images.unsplash.com/photo-1578985545062-69928b1d9587?q=80&w=500&auto=format&fit=crop" alt="Pastel">
                <h3>Muerte por Chocolate</h3>
                <p>$550.00</p>
                <button class="boton">Agregar al Carrito</button>
            </div>
            <div class="tarjeta">
                <img src="https://images.unsplash.com/photo-1464349095431-e9a21285b5f3?q=80&w=500&auto=format&fit=crop" alt="Pastel">
                <h3>Fresas con Crema</h3>
                <p>$480.00</p>
                <button class="boton">Agregar al Carrito</button>
            </div>
        </div>
    </section>

    <section id="rolls">
        <h2 class="seccion-titulo">🌀 Rolls Gourmet</h2>
        <div class="grid-productos">
            <div class="tarjeta">
                <img src="https://images.unsplash.com/photo-1509365465985-25d11c17e812?q=80&w=500&auto=format&fit=crop" alt="Roll">
                <h3>Cinnamon Roll Clásico</h3>
                <p>$65.00</p>
                <button class="boton">Agregar</button>
            </div>
        </div>
    </section>

    <section id="galletas">
        <h2 class="seccion-titulo">🍪 Galletas Artesanales (20+ Variedades)</h2>
        <div class="grid-productos">
            <div class="tarjeta">
                <img src="https://images.unsplash.com/photo-1499636138143-963773336891?q=80&w=500&auto=format&fit=crop" alt="Cookie">
                <h3>Chispas "Chunky"</h3>
                <p>$55.00</p>
                <button class="boton">Agregar</button>
            </div>
            <div class="tarjeta">
                <img src="https://images.unsplash.com/photo-1621236378699-8597fafedbd4?q=80&w=500&auto=format&fit=crop" alt="Cookie">
                <h3>Bomba de Avellana</h3>
                <p>$65.00</p>
                <button class="boton">Agregar</button>
            </div>
            <div class="tarjeta">
                <img src="https://images.unsplash.com/photo-1590080875515-8a3a8dc5735e?q=80&w=500&auto=format&fit=crop" alt="Cookie">
                <h3>Matcha Special</h3>
                <p>$70.00</p>
                <button class="boton">Agregar</button>
            </div>
            </div>
    </section>

    <section id="bebidas">
        <h2 class="seccion-titulo">☕ Bebidas</h2>
        <div class="grid-productos">
            <div class="tarjeta">
                <img src="https://images.unsplash.com/photo-1541167760496-162955ed8a9f?q=80&w=500&auto=format&fit=crop" alt="Bebida">
                <h3>Latte Vainilla</h3>
                <p>$75.00</p>
                <button class="boton">Agregar</button>
            </div>
            <div class="tarjeta">
                <img src="https://images.unsplash.com/photo-1461023058943-07fcbe16d735?q=80&w=500&auto=format&fit=crop" alt="Bebida">
                <h3>Frappé Mocha</h3>
                <p>$95.00</p>
                <button class="boton">Agregar</button>
            </div>
        </div>
    </section>

    <section id="visitanos">
        <h2 class="seccion-titulo">📍 Visítanos en nuestra sucursal</h2>
        <div class="ubicacion-contenedor">
            <div class="info-direccion">
                <h3>Nuestra Dirección:</h3>
                <p><strong>Privada San Miguel</strong></p>
                <p>Manzana 7, Lote 17, #162</p>
                <p>Colonia Misión San Agustín</p>
                <p>Estado de México, CP 55067</p>
                <hr>
                <p><strong>Horarios:</strong><br>Lunes a Sábado: 8:00 AM - 9:00 PM<br>Domingos: 9:00 AM - 8:00 PM</p>
                <p><strong>Teléfono:</strong> 55 1234 5678</p>
            </div>
            <div class="mapa-frame">
                <iframe 
                    src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d15037.123456789!2d-99.0185!3d19.5936!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x85d1f1f000000001%3A0x0!2zMTnCsDM1JzM3LjAiTiA5OcKwMDEnMDYuNiJX!5e0!3m2!1ses!2smx!4v1700000000000!5m2!1ses!2smx" 
                    allowfullscreen="" 
                    loading="lazy" 
                    referrerpolicy="no-referrer-when-downgrade">
                </iframe>
            </div>
        </div>
    </section>

</div>

<footer>
    <p><strong>Swete Crust S.A. de C.V.</strong></p>
    <p>Privada San Miguel Mz.7 Lt.17 #162 Col. Misión San Agustín</p>
    <p>&copy; 2026 Todos los derechos reservados.</p>
</footer>

</body>
</html>
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Swete Crust - Cotizador IA</title>
    <style>
        /* --- ESTILOS GENERALES DEL PROTOTIPO --- */
        body { font-family: 'Segoe UI', Roboto, Helvetica, Arial, sans-serif; margin: 0; background-color: #FFFACD; color: #333; scroll-behavior: smooth; }
        header { background-color: #fff; text-align: center; padding: 30px; border-bottom: 5px solid #FF4500; }
        .logo-nombre { color: #FF4500; font-size: 3.5em; margin: 0; font-family: 'Times New Roman', serif; font-style: italic; }
        nav { background-color: #FFD700; padding: 15px; text-align: center; position: sticky; top: 0; z-index: 1000; box-shadow: 0 2px 10px rgba(0,0,0,0.1); }
        nav a { text-decoration: none; color: #333; font-weight: bold; margin: 0 10px; padding: 10px 15px; border-radius: 25px; transition: 0.3s; }
        nav a:hover { background: #FF4500; color: #fff; }
        .container { max-width: 1100px; margin: 30px auto; background: #fff; padding: 30px; border-radius: 20px; box-shadow: 0 5px 20px rgba(0,0,0,0.08); }
        .seccion-titulo { text-align: center; color: #FF4500; font-size: 2.2em; border-bottom: 3px solid #FFD700; padding-bottom: 15px; margin-bottom: 30px; }

        /* --- ESTILOS ESPECÍFICOS DEL CHAT INTELIGENTE --- */
        .chat-contenedor { display: grid; grid-template-columns: 1fr; gap: 20px; }
        @media (min-width: 768px) { .chat-contenedor { grid-template-columns: 1fr 2fr; } }

        .info-lateral { background: #fff3cd; padding: 20px; border-radius: 15px; border: 2px solid #FFD700; }
        .info-lateral h3 { color: #FF4500; margin-top: 0; }

        .chat-box-frame { border: 1px solid #ddd; border-radius: 15px; overflow: hidden; display: flex; flex-direction: column; height: 500px; background: #f9f9f9; }
        .chat-header { background: linear-gradient(45deg, #FF4500, #ff7b00); color: white; padding: 15px; font-weight: bold; display: flex; align-items: center; font-size: 1.1em; }
        .chat-body { flex-grow: 1; padding: 20px; overflow-y: auto; display: flex; flex-direction: column; gap: 15px; scroll-behavior: smooth; }
        
        /* Mensajes */
        .mensaje { padding: 12px 18px; border-radius: 15px; max-width: 80%; line-height: 1.4; font-size: 0.95em; position: relative; }
        .mensaje-ia { align-self: flex-start; background: #e3f2fd; border-bottom-left-radius: 2px; border-left: 5px solid #2196F3; color: #0d47a1; }
        .mensaje-usuario { align-self: flex-end; background: #FF4500; color: white; border-bottom-right-radius: 2px; text-align: right; }
        
        .precio-estimado { display: inline-block; margin-top: 10px; padding: 5px 10px; background: #2e7d32; color: white; border-radius: 10px; font-weight: bold; font-size: 0.9em; }

        /* Área de entrada */
        .chat-input-area { display: flex; padding: 15px; background: #fff; border-top: 1px solid #eee; }
        .chat-input { flex-grow: 1; padding: 12px; border: 2px solid #ddd; border-radius: 25px; outline: none; transition: 0.3s; font-size: 1em; }
        .chat-input:focus { border-color: #FF4500; }
        .chat-btn { background: #FF4500; color: white; border: none; padding: 0 25px; margin-left: 10px; border-radius: 25px; cursor: pointer; font-weight: bold; font-size: 1em; transition: 0.3s; }
        .chat-btn:hover { background: #e63e00; transform: scale(1.05); }
    </style>
</head>
<body>

<header>
    <h1 class="logo-nombre">🍪 Swete Crust AI ❤️</h1>
    <p>Tu asistente virtual de repostería</p>
</header>

<nav>
    <a href="#">🏠 Inicio</a>
    <a href="#cotizador">🤖 Cotizador Inteligente</a>
    <a href="#">📍 Contacto</a>
</nav>

<div class="container" id="cotizador">
    <h2 class="seccion-titulo">✨ Asistente de Pedidos y Cotizaciones</h2>
    
    <div class="chat-contenedor">
        <div class="info-lateral">
            <h3>💡 ¿Cómo funciona?</h3>
            <p>Describe tu idea y nuestra IA te dará sugerencias y un precio aproximado al instante.</p>
            <p><strong>Ejemplos de qué decirle:</strong></p>
            <ul>
                <li>"Quiero un pastel de chocolate para 20 personas"</li>
                <li>"Busco algo elegante para una boda civil"</li>
                <li>"Necesito galletas de avena saludables"</li>
                <li>"Un pastel de fresas para cumpleaños de niño"</li>
            </ul>
            <p style="font-size: 0.9em; color: #666;">*Los precios son estimados y pueden variar según el diseño final.</p>
        </div>

        <div class="chat-box-frame">
            <div class="chat-header">
                <span style="font-size: 1.5em; margin-right: 10px;">👩‍🍳</span> SweteBot - Asistente Pastelero
            </div>
            
            <div class="chat-body" id="cuerpoChat">
                <div class="mensaje mensaje-ia">
                    ¡Hola! Soy la IA de Swete Crust. 👋 Cuéntame qué se te antoja hoy y te ayudaré con ideas y precios aproximados.
                </div>
            </div>
            
            <div class="chat-input-area">
                <input type="text" id="inputUsuario" class="chat-input" placeholder="Escribe aquí tu idea... (ej. pastel de boda)" onkeypress="verificarEnter(event)">
                <button class="chat-btn" onclick="procesarMensaje()">Enviar ➤</button>
            </div>
        </div>
    </div>

</div>

<script>
    // --- LÓGICA DE "INTELIGENCIA ARTIFICIAL" SIMULADA ---
    function analizarTextoIA(texto) {
        let t = texto.toLowerCase(); // Convertir todo a minúsculas para analizar
        let respuesta = "";
        let precio = "";

        // 1. Detección de Eventos Grandes (Boda/XV Años)
        if (t.includes("boda") || t.includes("matrimonio") || t.includes("elegante") || t.includes("pisos")) {
            respuesta = "¡Qué emoción! Para una ocasión tan especial, sugiero un diseño de 2 o 3 pisos con cubierta de fondant alisado, detalles en encaje comestible o flores naturales para un toque sofisticado.";
            precio = "Rango estimado: $850 - $1,800 MXN (según tamaño y decoración).";
        } 
        // 2. Detección de Amantes del Chocolate
        else if (t.includes("chocolate") || t.includes("nutella") || t.includes("ferrero") || t.includes("cacao")) {
            respuesta = "¡Excelente elección! Para los amantes del cacao, podemos hacer un bizcocho súper húmedo de chocolate oscuro, relleno de ganache de Nutella y decorado con trufas artesanales arriba.";
            precio = "Rango estimado: $550 - $700 MXN.";
        }
        // 3. Detección de Frutas / Frescura
        else if (t.includes("fresa") || t.includes("fruta") || t.includes("mango") || t.includes("limon") || t.includes("fresco")) {
            respuesta = "Una opción deliciosa y ligera. Te propongo un bizcocho de vainilla humedecido con tres leches, relleno de crema chantilly y trozos abundantes de fruta de temporada.";
            precio = "Rango estimado: $450 - $600 MXN.";
        }
        // 4. Detección de Cumpleaños / Niños
        else if (t.includes("cumpleaños") || t.includes("fiesta") || t.includes("niño") || t.includes("niña") || t.includes("color")) {
            respuesta = "¡Celebración en puerta! 🎉 Podemos hacerlo muy divertido con masa tipo 'funfetti' (chispas de colores por dentro) y una decoración vibrante con el tema o personaje que prefieras en betún de mantequilla.";
            precio = "Rango estimado: $500 - $750 MXN.";
        }
        // 5. Detección de Saludable / Galletas
        else if (t.includes("saludable") || t.includes("avena") || t.includes("integral") || t.includes("sin azucar") || t.includes("galleta")) {
            respuesta = "¡Claro! En Swete Crust cuidamos tu salud. Tenemos opciones increíbles de galletas de avena con miel y pasas, o pasteles con harina integral y endulzados con stevia/monk fruit.";
            precio = "Rango estimado: $60 MXN (por galleta jumbo) o $400 MXN (pastel chico).";
        }
        // 6. Respuesta Genérica (si no entiende)
        else {
            respuesta = "¡Suena interesante! Para poder darte una idea más creativa y un precio exacto, ¿podrías decirme para cuántas personas sería o qué sabor principal te gustaría?";
            precio = "Pendiente de más detalles para cotizar.";
        }

        return { msj: respuesta, costo: precio };
    }

    // --- FUNCIONES DE INTERFAZ DE CHAT ---
    function procesarMensaje() {
        let input = document.getElementById("inputUsuario");
        let texto = input.value.trim();
        if (texto === "") return;

        let chatBody = document.getElementById("cuerpoChat");

        // 1. Mostrar mensaje del usuario
        let userBubble = document.createElement("div");
        userBubble.className = "mensaje mensaje-usuario";
        userBubble.innerText = texto;
        chatBody.appendChild(userBubble);
        input.value = ""; // Limpiar input
        scrollAlFondo();

        // 2. Analizar texto con la "IA"
        let analisis = analizarTextoIA(texto);

        // 3. Simular tiempo de espera ("escribiendo...")
        setTimeout(() => {
            let iaBubble = document.createElement("div");
            iaBubble.className = "mensaje mensaje-ia";
            // Insertamos el mensaje y el precio en HTML
            iaBubble.innerHTML = Isabel (IA) dice:<br>${analisis.msj}<br><div class="precio-estimado">💰 ${analisis.costo}</div>;
            chatBody.appendChild(iaBubble);
            scrollAlFondo();
        }, 700); // 0.7 segundos de retraso para realismo
    }

    function scrollAlFondo() {
        let chatBody = document.getElementById("cuerpoChat");
        chatBody.scrollTop = chatBody.scrollHeight;
    }

    function verificarEnter(event) {
        if (event.key === "Enter") {
            procesarMensaje();
        }
    }
</script>

</body>
</html>
