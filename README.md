<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <title>***Autolavado “TuLavado”***</title>
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <style>
    :root {
      --negro: #000;
      --blanco: #fff;
      --gris: #f5f5f5;
    }
    * {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
    }
    body {
      font-family: Arial, Helvetica, sans-serif;
      background: var(--blanco);
      color: var(--negro);
      line-height: 1.6;
    }
    header {
      background: var(--negro);
      color: var(--blanco);
      padding: 2rem 1rem;
      text-align: center;
    }
    header h1 {
      font-size: 2rem;
      letter-spacing: 2px;
    }
    header p {
      margin-top: 0.5rem;
      font-size: 1.1rem;
    }
    nav {
      background: var(--gris);
      padding: 1rem;
      text-align: center;
    }
    nav a {
      color: var(--negro);
      text-decoration: none;
      margin: 0 1rem;
      font-weight: bold;
      border-bottom: 2px solid transparent;
      transition: border-color 0.3s;
    }
    nav a:focus, nav a:hover {
      border-color: var(--negro);
      outline: none;
    }
    section {
      padding: 3rem 1rem;
      max-width: 900px;
      margin: auto;
    }
    h2 {
      margin-bottom: 1rem;
      text-align: center;
      font-size: 1.8rem;
    }
    .galeria {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
      gap: 1rem;
      margin-top: 2rem;
    }
    .galeria img {
      width: 100%;
      height: 200px;
      object-fit: cover;
      border: 2px solid var(--negro);
    }
    .btn-wa {
      display: inline-block;
      background: var(--negro);
      color: var(--blanco);
      padding: 1rem 2rem;
      margin: 2rem 0;
      text-decoration: none;
      border-radius: 4px;
      font-weight: bold;
      transition: background 0.3s;
    }
    .btn-wa:focus, .btn-wa:hover {
      background: #333;
    }
    form {
      display: grid;
      gap: 1rem;
      max-width: 500px;
      margin: auto;
    }
    input, textarea, button {
      padding: 0.75rem;
      font-size: 1rem;
      border: 2px solid var(--negro);
      background: var(--blanco);
      color: var(--negro);
    }
    button {
      cursor: pointer;
      font-weight: bold;
    }
    footer {
      text-align: center;
      padding: 2rem 1rem;
      background: var(--negro);
      color: var(--blanco);
    }
    /* Accesibilidad extra */
    @media (prefers-reduced-motion: reduce) {
      * {
        transition: none !important;
      }
    }
  </style>
</head>
<body>

  <header>
    <h1>***Autolavado “TuLavado”***</h1>
    <p>Limpieza impecable con atención de primer nivel</p>
  </header>

  <nav aria-label="Menú principal">
    <a href="#servicios">Servicios</a>
    <a href="#galeria">Galería</a>
    <a href="#agenda">Agenda tu cita</a>
    <a href="#contacto">Contacto</a>
  </nav>

  <section id="servicios">
    <h2>Nuestros servicios</h2>
    <ul>
      <li>Lavado exterior e interior</li>
      <li>Aspirado profundo</li>
      <li>Encerado y pulido</li>
      <li>Limpieza de motor</li>
      <li>Desinfección de ozono</li>
    </ul>
  </section>

  <section id="galeria">
    <h2>Antes y después</h2>
    <div class="galeria">
      <!-- Reemplaza src y alt con tus propias fotos -->
      <img src="foto1.jpg" alt="Auto muy sucio antes del lavado">
      <img src="foto2.jpg" alt="Auto brillante después del lavado">
      <img src="foto3.jpg" alt="Interior del auto limpio">
    </div>
  </section>

  <section id="agenda">
    <h2>Agenda tu cita por WhatsApp</h2>
    <p>Haz clic en el botón o escríbenos directamente.</p>
    <a class="btn-wa" href="https://wa.me/***549123456789***?text=Hola,%20quiero%20agendar%20una%20cita%20para%20lavar%20mi%20auto" target="_blank" rel="noopener noreferrer">Reservar por WhatsApp</a>
  </section>

  <section id="contacto">
    <h2>O déjanos un mensaje</h2>
    <form action="https://formsubmit.co/***tu@email.com***" method="POST">
      <label for="nombre">Nombre</label>
      <input type="text" id="nombre" name="nombre" required>

      <label for="tel">Teléfono</label>
      <input type="tel" id="tel" name="tel" required>

      <label for="mensaje">Mensaje</label>
      <textarea id="mensaje" name="mensaje" rows="4" required></textarea>

      <button type="submit">Enviar mensaje</button>
    </form>
  </section>

  <footer>
    <p>Dirección: ***Calle 123, Ciudad***</p>
    <p>Horario: L a V 9–18 h | Sáb 9–13 h</p>
    <p>Teléfono: ***123 456 789***</p>
  </footer>

</body>
</html>
