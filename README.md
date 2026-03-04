# Tienda-Tecnolog-ca
Hola bienvenido al emprendimiento estamos trabajando para que sea rápido y seguro🌐
<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Tienda Tech Pro</title>
  <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600;700&display=swap" rel="stylesheet">
  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
      font-family: 'Poppins', sans-serif;
    }

    body {
      background: #0f172a;
      color: #f1f5f9;
    }

    header {
      display: flex;
      justify-content: space-between;
      align-items: center;
      padding: 20px 8%;
      background: rgba(15, 23, 42, 0.9);
      backdrop-filter: blur(10px);
      position: sticky;
      top: 0;
      z-index: 1000;
    }

    header h1 {
      font-size: 26px;
      font-weight: 700;
      background: linear-gradient(90deg, #38bdf8, #6366f1);
      -webkit-background-clip: text;
      -webkit-text-fill-color: transparent;
    }

    nav a {
      color: #cbd5e1;
      text-decoration: none;
      margin-left: 25px;
      font-weight: 500;
      transition: 0.3s;
    }

    nav a:hover {
      color: #38bdf8;
    }

    .hero {
      text-align: center;
      padding: 100px 20px;
      background: radial-gradient(circle at top, #1e293b, #0f172a);
    }

    .hero h2 {
      font-size: 42px;
      margin-bottom: 15px;
    }

    .hero p {
      font-size: 18px;
      color: #94a3b8;
    }

    .productos {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
      gap: 30px;
      padding: 60px 8%;
    }

    .card {
      background: #1e293b;
      padding: 20px;
      border-radius: 20px;
      box-shadow: 0 10px 30px rgba(0,0,0,0.4);
      text-align: center;
      transition: 0.4s ease;
    }

    .card:hover {
      transform: translateY(-10px);
      box-shadow: 0 20px 40px rgba(0,0,0,0.6);
    }

    .card img {
      width: 100%;
      height: 220px;
      object-fit: cover;
      border-radius: 15px;
      margin-bottom: 15px;
    }

    .card h3 {
      font-size: 20px;
      margin-bottom: 10px;
    }

    .precio {
      font-size: 22px;
      font-weight: 600;
      margin-bottom: 15px;
      color: #38bdf8;
    }

    button {
      background: linear-gradient(90deg, #6366f1, #38bdf8);
      color: white;
      border: none;
      padding: 12px 20px;
      border-radius: 30px;
      cursor: pointer;
      font-weight: 600;
      transition: 0.3s;
    }

    button:hover {
      opacity: 0.8;
    }

    footer {
      text-align: center;
      padding: 30px;
      background: #0f172a;
      border-top: 1px solid #1e293b;
      color: #64748b;
    }
  </style>
</head>
<body>

<header>
  <h1>Tienda Tech</h1>
  <nav>
    <a href="#">Inicio</a>
    <a href="#productos">Productos</a>
    <a href="#contacto">Contacto</a>
  </nav>
</header>

<section class="hero">
  <h2>Tecnología que marca la diferencia</h2>
  <p>Innovación, potencia y estilo en un solo lugar</p>
</section>

<section class="productos" id="productos">
  <div class="card">
    <img src="https://via.placeholder.com/400x300" alt="Laptop Gamer">
    <h3>Laptop Gamer</h3>
    <p class="precio">$1200</p>
    <button onclick="agregarAlCarrito('Laptop Gamer')">Agregar al carrito</button>
  </div>

  <div class="card">
    <img src="https://via.placeholder.com/400x300" alt="Auriculares Bluetooth">
    <h3>Auriculares Bluetooth</h3>
    <p class="precio">$150</p>
    <button onclick="agregarAlCarrito('Auriculares Bluetooth')">Agregar al carrito</button>
  </div>

  <div class="card">
    <img src="https://via.placeholder.com/400x300" alt="Smartphone Pro">
    <h3>Smartphone Pro</h3>
    <p class="precio">$900</p>
    <button onclick="agregarAlCarrito('Smartphone Pro')">Agregar al carrito</button>
  </div>
</section>

<footer id="contacto">
  <p>© 2026 Tienda Tech - Todos los derechos reservados</p>
  <p>Contacto: contacto@tiendatech.com</p>
</footer>

<script>
  function agregarAlCarrito(producto) {
    alert(producto + " agregado al carrito 🛒");
  }
</script>

</body>
</html>
