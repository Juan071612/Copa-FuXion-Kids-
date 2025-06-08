# Copa-FuXion-Kids-
<!DOCTYPE html>
<html lang="es">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1" />
<title>Copa Fuxion Kids | Torneo Infantil</title>
<style>
  /* Reset básico */
  *, *::before, *::after {
    margin: 0; padding: 0; box-sizing: border-box;
  }
  body {
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    background: linear-gradient(135deg, #006400, #a1c935);
    color: #fff;
    min-height: 100vh;
    display: flex;
    flex-direction: column;
  }
  header {
    background-color: #004d00;
    padding: 1.5rem 1rem;
    display: flex;
    justify-content: space-between;
    align-items: center;
    flex-wrap: wrap;
    box-shadow: 0 4px 6px rgba(0,0,0,0.3);
  }
  header h1 {
    font-size: 1.6rem;
    font-weight: 700;
    letter-spacing: 2px;
  }
  nav {
    display: flex;
    flex-wrap: wrap;
  }
  nav a {
    color: #cfe396;
    margin-left: 1rem;
    text-decoration: none;
    font-weight: 600;
    transition: color 0.3s ease;
  }
  nav a:hover,
  nav a:focus {
    color: #e9f7d5;
    outline: none;
  }
  main {
    flex: 1;
    padding: 2rem 1rem;
    max-width: 900px;
    margin: 0 auto 2rem;
    background: rgba(0, 77, 0, 0.85);
    border-radius: 12px;
    box-shadow: 0 6px 10px rgba(0,0,0,0.5);
  }
  section {
    margin-bottom: 2rem;
  }
  h2 {
    font-size: 1.8rem;
    margin-bottom: 1rem;
    color: #d4edda;
    text-align: center;
    text-shadow: 1px 1px 3px #014d01;
  }
  p, ul {
    font-size: 1rem;
    line-height: 1.5;
  }
  ul {
    list-style-type: square;
    padding-left: 1.5rem;
    margin-top: 0.5rem;
  }
  .frase-motivadora {
    font-style: italic;
    text-align: center;
    margin-bottom: 2rem;
    font-weight: 700;
    color: #d4edda;
    text-shadow: 2px 2px 5px #014d01;
  }
  form {
    background: #004d00;
    padding: 1.5rem;
    border-radius: 12px;
    box-shadow: inset 0 0 10px #82c91e;
  }
  label {
    display: block;
    margin-bottom: 0.4rem;
    font-weight: 600;
  }
  input, select {
    width: 100%;
    padding: 0.5rem;
    border-radius: 6px;
    border: none;
    margin-bottom: 1rem;
    font-size: 1rem;
  }
  input[type="submit"] {
    background: #a1c935;
    color: #004d00;
    font-weight: 700;
    border: none;
    cursor: pointer;
    transition: background 0.3s ease;
    padding: 1rem;
    border-radius: 8px;
  }
  input[type="submit"]:hover,
  input[type="submit"]:focus {
    background: #83b720;
    outline: none;
  }
  footer {
    background: #004d00;
    padding: 1rem 1rem;
    text-align: center;
    color: #cfe396;
    font-size: 0.9rem;
    box-shadow: 0 -3px 6px rgba(0,0,0,0.3);
  }
  footer a {
    color: #d4edda;
    text-decoration: none;
    margin: 0 0.3rem;
    font-weight: 600;
  }
  footer a:hover,
  footer a:focus {
    text-decoration: underline;
    outline: none;
  }

  /* Responsive */
  @media (max-width: 600px) {
    header {
      flex-direction: column;
      align-items: flex-start;
    }
    nav {
      margin-top: 0.5rem;
      width: 100%;
      justify-content: space-around;
    }
    nav a {
      margin-left: 0;
      padding: 0.3rem 0.5rem;
      flex: 1 1 auto;
      text-align: center;
    }
  }
</style>
</head>
<body>

<header>
  <h1>Copa Fuxion Kids</h1>
  <nav aria-label="Menú principal">
    <a href="#info">Información</a>
    <a href="#categoria">Categoría</a>
    <a href="#inscripcion">Inscripción</a>
    <a href="#contacto">Contacto</a>
  </nav>
</header>

<main>
  <section id="info" tabindex="0">
    <h2>¡Bienvenidos a la Copa Fuxion Kids!</h2>
    <p>Un torneo infantil donde los niños no solo juegan fútbol, sino que también aprenden valores como la disciplina, el trabajo en equipo y el amor por el deporte y la vida saludable.</p>
    <p>Organizado por <strong>Fuxion</strong>, promovemos la energía y el bienestar para que nuestros futuros cracks crezcan sanos y fuertes.</p>
  </section>

  <div class="frase-motivadora" aria-live="polite">
    “Del barrio para la fama, aquí no se pierde, aquí se gana.”
  </div>

  <section id="categoria" tabindex="0">
    <h2>Categoría Única</h2>
    <ul>
      <li>10 a 13 años</li>
    </ul>
  </section>

  <section id="beneficios" tabindex="0">
    <h2>Beneficios para los participantes</h2>
    <ul>
      <li>Productos Fuxion para mejorar la energía y concentración</li>
      <li>Entrenamientos especializados con entrenadores profesionales</li>
      <li>Medallas y trofeos para los mejores equipos y jugadores destacados</li>
      <li>Actividades recreativas y educativas para todos los niños</li>
    </ul>
  </section>

  <section id="inscripcion" tabindex="0">
    <h2>Inscripción</h2>
    <p>¡No dejés que tu pequeño crack se quede por fuera! Inscribilo ya y dale la oportunidad de vivir la experiencia Fuxion.</p>
    <form id="formInscripcion" aria-label="Formulario de inscripción">
      <label for="nombre">Nombre del niño:</label>
      <input type="text" id="nombre" name="nombre" required placeholder="Juan Pérez" autocomplete="off" />

      <label for="edad">Edad:</label>
      <select id="edad" name="edad" required>
        <option value="" disabled selected>Seleccioná la edad</option>
        <option value="10-13">10-13 años</option>
      </select>

      <label for="equipo">Equipo favorito:</label>
      <select id="equipo" name="equipo" required>
        <option value="" disabled selected>Seleccioná el equipo</option>
        <option value="atletico_nacional">Atlético Nacional (máx. 11 jugadores)</option>
        <option value="america_de_cali">América de Cali (máx. 11 jugadores)</option>
        <option value="independiente_medellin">Independiente Medellín (máx. 11 jugadores)</option>
        <option value="millonarios">Millonarios (máx. 11 jugadores)</option>
        <option value="deportivo_cali">Deportivo Cali (máx. 11 jugadores)</option>
        <option value="junior">Junior de Barranquilla (máx. 11 jugadores)</option>
        <option value="once_caldas">Once Caldas (máx. 11 jugadores)</option>
        <option value="tolima">Deportes Tolima (máx. 11 jugadores)</option>
      </select>

      <label for="padre">Nombre del padre o madre:</label>
      <input type="text" id="padre" name="padre" required placeholder="Carlos Gómez" autocomplete="off" />

      <label for="contacto">Teléfono o WhatsApp:</label>
      <input type="tel" id="contacto" name="contacto" required placeholder="+57 316 0431887" autocomplete="off" pattern="\+?\d[\d\s\-]{7,}" title="Número válido, ejemplo: +57 316 0431887" />

      <input type="submit" value="Enviar Inscripción" />
    </form>
  </section>

  <section id="contacto" tabindex="0">
    <h2>Contacto</h2>
    <p>Para más información, escribinos a:</p>
    <p><strong>WhatsApp:</strong> +57 316 0431887 </p>
   
    <p>Síguenos en nuestras redes para estar al día con todas las noticias de la Copa Fuxion Kids:</p>
    <p>
      <a href="https://facebook.com/fuxionkids" target="_blank" rel="noopener noreferrer">Facebook
