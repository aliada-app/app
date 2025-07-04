<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>ALIADA</title>
  <style>
    body {
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
      background-color: #f9fdfb;
      color: #333;
      margin: 0;
      padding: 0 20px 40px;
      line-height: 1.6;
    }
    header {
      background-color: #4caf50;
      color: white;
      padding: 30px 20px;
      text-align: center;
      box-shadow: 0 2px 5px rgba(0,0,0,0.1);
    }
    header h1 {
      margin: 0 0 10px;
      font-size: 3rem;
      letter-spacing: 3px;
    }
    header p {
      font-size: 1.3rem;
      margin: 0;
      font-weight: 500;
    }
    .buttons {
      margin: 20px 0;
      text-align: center;
      gap: 20px;
      display: flex;
      justify-content: center;
      flex-wrap: wrap;
    }
    button, .btn-link {
      background-color: #e53935;
      border: none;
      color: white;
      padding: 15px 25px;
      font-size: 1.1rem;
      border-radius: 5px;
      cursor: pointer;
      transition: background-color 0.3s ease;
      text-decoration: none;
      display: inline-block;
      user-select: none;
    }
    button:hover, .btn-link:hover {
      background-color: #b71c1c;
    }
    .btn-link {
      background-color: #1976d2;
    }
    .btn-link:hover {
      background-color: #0d47a1;
    }
    section {
      max-width: 900px;
      margin: 40px auto;
      background: white;
      padding: 25px 30px;
      border-radius: 8px;
      box-shadow: 0 3px 8px rgba(0,0,0,0.1);
    }
    section h2 {
      color: #4caf50;
      margin-bottom: 15px;
      border-bottom: 3px solid #4caf50;
      padding-bottom: 5px;
    }
    section p, section ul {
      margin-bottom: 15px;
    }
    ul {
      padding-left: 20px;
    }
    .emoji {
      font-size: 1.2rem;
      margin-right: 6px;
    }
    /* Test styles */
    .test-question {
      margin-bottom: 12px;
      font-weight: 600;
    }
    .test-options label {
      margin-right: 20px;
      cursor: pointer;
    }
    #result {
      margin-top: 20px;
      font-weight: 700;
      font-size: 1.1rem;
      color: #333;
    }
    /* Fundaciones list */
    .fundacion {
      margin-bottom: 15px;
    }
    .fundacion strong {
      color: #2e7d32;
    }
    /* Responsive */
    @media (max-width: 600px) {
      header h1 {
        font-size: 2.2rem;
      }
      button, .btn-link {
        width: 100%;
        margin-bottom: 10px;
      }
      .buttons {
        flex-direction: column;
      }
    }
  </style>
</head>
<body>

  <header>
    <h1>ALIADA</h1>
    <p>Bienvenida a tu comunidad de Paz y armonía</p>
  </header>

  <div class="buttons">
    <button onclick="llamar911()">🚨 Llamar al 911</button>
    <a href="#informacion" class="btn-link">➡️ Ir a Información</a>
  </div>

  <section id="informacion">
    <h2>Información sobre ALIADA</h2>
    <p><strong>ALIADA</strong> es una aplicación pensada para mujeres que enfrentan violencia. Combina ayuda inmediata, educación y herramientas prácticas para actuar y prevenir.</p>

    <p><span class="emoji">📚</span><strong>Contenido educativo</strong></p>

    <p><strong>¿Qué es la violencia de género?</strong> Toda acción o amenaza de acción que cause daño físico, sexual, psicológico o privación de libertad a una mujer por el hecho de serlo, y que se origina en relaciones desiguales de poder entre hombres y mujeres.</p>

    <p><strong>Tipos de violencia:</strong></p>
    <ul>
      <li><strong>Física:</strong> Golpes, empujones.</li>
      <li><strong>Psicológica:</strong> Humillaciones, amenazas.</li>
      <li><strong>Sexual:</strong> Actos forzados sin consentimiento.</li>
      <li><strong>Económica:</strong> Control del dinero o recursos.</li>
      <li><strong>Digital:</strong> Acoso o control por redes sociales.</li>
    </ul>

    <p><strong>Ámbitos de la violencia:</strong> Espacios donde puede ocurrir: hogar, escuela, trabajo, redes sociales, comunidad.</p>

    <p><strong>Ciclo de la violencia:</strong> Fases que se repiten: acumulación de tensión → agresión → reconciliación (“luna de miel”).</p>

    <p><strong>¿Cómo salir del círculo?</strong> Buscar ayuda, hacer un plan de escape, hablar con alguien de confianza, usar la app.</p>

    <p><strong>Relaciones sanas vs tóxicas:</strong> Amor sano implica respeto, empatía y consentimiento. La violencia no es amor.</p>

    <p><strong>Señales de alerta:</strong> Celos excesivos, aislamiento, control, insultos. Incluye test de autoevaluación.</p>
  </section>

  <section id="test">
    <h2>TEST DE AUTOEVALUACIÓN</h2>
    <p>Responde <strong>SÍ</strong> o <strong>NO</strong> a las siguientes preguntas:</p>

    <form id="testForm">
      <div class="test-question">
        1. ¿Tu pareja controla con quién hablas o a dónde vas?
        <div class="test-options">
          <label><input type="radio" name="q1" value="sí" required> Sí</label>
          <label><input type="radio" name="q1" value="no"> No</label>
        </div>
      </div>

      <div class="test-question">
        2. ¿Te revisa el celular, redes sociales o te exige tus contraseñas?
        <div class="test-options">
          <label><input type="radio" name="q2" value="sí" required> Sí</label>
          <label><input type="radio" name="q2" value="no"> No</label>
        </div>
      </div>

      <div class="test-question">
        3. ¿Te insulta, humilla o menosprecia, incluso en público?
        <div class="test-options">
          <label><input type="radio" name="q3" value="sí" required> Sí</label>
          <label><input type="radio" name="q3" value="no"> No</label>
        </div>
      </div>

      <div class="test-question">
        4. ¿Te hace sentir culpable por todo lo que sale mal?
        <div class="test-options">
          <label><input type="radio" name="q4" value="sí" required> Sí</label>
          <label><input type="radio" name="q4" value="no"> No</label>
        </div>
      </div>

      <div class="test-question">
        5. ¿Se enoja si pasas tiempo con tu familia o amistades?
        <div class="test-options">
          <label><input type="radio" name="q5" value="sí" required> Sí</label>
          <label><input type="radio" name="q5" value="no"> No</label>
        </div>
      </div>

      <div class="test-question">
        6. ¿Te ha empujado, golpeado o amenazado con hacerlo?
        <div class="test-options">
          <label><input type="radio" name="q6" value="sí" required> Sí</label>
          <label><input type="radio" name="q6" value="no"> No</label>
        </div>
      </div>

      <div class="test-question">
        7. ¿Te obliga a tener relaciones sexuales o te presiona cuando no quieres?
        <div class="test-options">
          <label><input type="radio" name="q7" value="sí" required> Sí</label>
          <label><input type="radio" name="q7" value="no"> No</label>
        </div>
      </div>

      <button type="submit" style="background-color:#4caf50; margin-top:15px;">Calificar Test</button>
    </form>

    <div id="result" aria-live="polite"></div>
  </section>

  <section id="fundaciones">
    <h2>Fundaciones de Apoyo a Nivel Nacional</h2>

    <div class="fundacion">
      <strong>Azuay</strong><br />
      Centro de apoyo a la Mujer y a la familia ‘Las Marías’: Dirección: Benigno Malo y Vega Muñoz, Teléfono: 0979186468 / Correo: lasmariascuencatrabajosocial@gmail.com, lasmariascuencalegal@gmail.com<br />
      Fundación María Amor (Cuenca): 095 893 4487 / (07)2832817 – correo: lineadeapoyoamujeres@gmail.com<br />
      Casa de la Mujer: Dirección: General Torres 7-45 y Presidente Córdova. Cuenca / Teléfono: 07 4134900 Ext. 2345 / Correo: abzambrano@cuenca.gob.ec
    </div>

    <div class="fundacion">
      <strong>Manabí</strong><br />
      Fundación Nuevos Horizontes (Chone): 099 352 0358 (Portoviejo): 099 352 0358 / Correo: funhor@hotmail.com<br />
      Centro Matilde Santa Marta “Atención Inicial Integral para Mujeres Víctimas de Violencia” (Portoviejo): Dirección: Av. Universitaria y Aljhuela / Correo: fundacion_santa_marta@yahoo.com<br />
      Fundación Río Manta: Dirección: Calle Efraín Alava y 9 de Octubre. Barrio Miraflores / Teléfono: (05) 2926 236 / Correo: fundacionriomanta@hotmail.com<br />
      Fundación Nuevos Horizontes: Dirección: Calle Mejía, entre Bolívar y Quiroga / Teléfono: 099 352 0358 – 093 946 7066 / Correo: funhor@hotmail.com
    </div>

    <div class="fundacion">
      <strong>Bolívar - Guaranda</strong><br />
      Foro Provincial de la Mujer de Bolívar:<br />
      Asesoría legal: 099 614 6137 / 098 196 2215<br />
      Asesoría psicológica: 097 969 8169
    </div>

    <div class="fundacion">
      <strong>Carchi - Tulcán</strong><br />
      AVSI: 093 914 4461<br />
      HIAS: 096 316 1400 / 023 825 770<br />
      Fundación Lunita Lunera: 096 859 2806<br />
      Fundación Alas de Colibrí: 095 989 0029<br />
      ACNUR: 098 820 5907
    </div>

    <div class="fundacion">
      <strong>Cañar - Azogues</strong><br />
      Fundación Solidaridad y Familia: Teléfono: 07 224 6943 / Dirección 1: Calle Bolívar 2-05 entre Azuay y Veintimilla – Dirección 2: Calle 3 de noviembre y Colón / Correo: sofamifundacion@gmail.com
    </div>

    <div class="fundacion">
      <strong>Sucumbíos</strong><br />
      Federación de Mujeres de Sucumbíos: 098 600 5724<br />
      Centro Puerta Violeta de la Federación de Mujeres de Sucumbíos: 099 207 1726<br />
      Fundación Lunita Lunera: 099 716 6186<br />
      Centro Violeta del Ministerio de la Mujer: Av. Circunvalación y Av. Monseñor Leonidas Proaño, edificio Centro de Atención Ciudadana (CAC)<br />
      Alas de Colibrí: 098 466 8316<br />
      OIM: 099 411 2640 / 098 927 3791
    </div>

    <div class="fundacion">
      <strong>Pichincha</strong><br />
      COINCAD (Cayambe): 02 2110 220<br />
      Casa de la Mujer: 1800 288 523<br />
      Fundación Casa de Refugio Matilde: 099 669 6723 / 098 779 6688 / (02) 262 7591 / (02) 262 5316<br />
      Fundación Nuestros Jóvenes (Quito): 098 780 5409 / 099 910 7227<br />
      Surkuna: 096 363 0034 / info@surkuna.org<br />
      Warmi Pichincha: 098 742 7448 / Línea directa: 166<br />
      CEPAM: 098 838 2526 / 099 268 5614 / info@cepam.org.ec<br />
      Akuanuna: 096 351 6891
    </div>

    <div class="fundacion">
      <strong>Chimborazo</strong><br />
      Fundación Nosotras con Equidad: 098 427 7871
    </div>

    <div class="fundacion">
      <strong>El Oro</strong><br />
      Movimiento de Mujeres de El Oro (Machala): 098 948 6451<br />
      Centro de Derechos Humanos (Huaquillas): 096 789 8963
    </div>

    <div class="fundacion">
      <strong>Esmeraldas</strong><br />
      Fundación Foro de Desarrollo Integral de la Mujer y la Familia: 098 138 3463 / (06) 270 0757<br />
      Centro Violeta MMDH: Av. Jaime Roldós, Puerto Pesquero Artesanal del cantón Esmeraldas. Ed. del Centro de Atención Ciudadana (CAC)
    </div>

    <div class="fundacion">
      <strong>Guayas</strong><br />
      CEPAM: 099 4151 219 / info@cepam.org.ec<br />
      CDH: (04) 229 3931 / (04) 229 3273 / cdh@cdh.org.ec<br />
      Fundación Estudios y Apoyo para la Mujer y la Familia Ecuatoriana María Guare: 098 432 2193<br />
      Fundación Mujer y Mujer: 096 387 4624 / Esmeraldas 901 y Av. 9 de octubre / infomym.gye@gmail.com
    </div>

    <div class="fundacion">
      <strong>Ibarra</strong><br />
      Alas de Colibrí: 096 411 0602<br />
      Asociación ASIRIS: 098 331 6787<br />
      Cemoplaf: Rocafuerte 9-60 y Colón / 06 295 9918 – 099 503 5325
    </div>

    <div class="fundacion">
      <strong>Machala</strong><br />
      Movimiento de Mujeres del Oro: 098 948 6451<br />
      Fundación Quimera: quimera96@yahoo.com<br />
      PLAPERTS: 098 170 7205
    </div>

    <div class="fundacion">
      <strong>Tena</strong><br />
      Casa Wasi Pani Tena: 098 732 9945
    </div>

    <div class="fundacion">
      <strong>Santa Elena</strong><br />
      Casa Hogar de Nazareth: 099 530 6609 / 099 336 0042
    </div>

    <div class="fundacion">
      <strong>Santo Domingo</strong><br />
      CEPAM: 099 4151 219 / info@cepam.org.ec<br />
      CDH: (04) 229 3931 / (04) 229 3273 / cdh@cdh.org.ec<br />
      Fundación Estudios y Apoyo para la Mujer y la Familia Ecuatoriana María Guare: 098 432 2193<br />
      Fundación Mujer y Mujer: 096 387 4624 / Esmeraldas 901 y Av. 9 de octubre / infomym.gye@gmail.com
    </div>

    <div class="fundacion">
      <strong>Orellana</strong><br />
      Fundación Ayllu Huarmicucha, Casa Paula: 06 288 1917<br />
      Centro de atención externa de la Fundación Ayllu Huarmicucha: 06 2302 353
    </div>
  </section>

  <script>
    function llamar911() {
      // Intentar llamar al 911 (solo funciona en dispositivos que soportan tel:)
      window.location.href = "tel:911";
    }

    document.getElementById('testForm').addEventListener('submit', function (e) {
      e.preventDefault();

      // Obtener respuestas
      const respuestas = [];
      for (let i = 1; i <= 7; i++) {
        const val = document.querySelector(`input[name="q${i}"]:checked`).value.toLowerCase();
        respuestas.push(val);
      }

      // Contar respuestas "sí"
      const totalSi = respuestas.filter(r => r === 'sí').length;

      let mensaje = "";
      if (totalSi <= 2) {
        mensaje = "Tu relación puede tener desacuerdos, pero no hay señales claras de violencia. Aun así, mantente atenta y cuida tus límites personales.";
      } else if (totalSi >= 3 && totalSi <= 5) {
        mensaje = "Hay varias señales de alerta. Puede que estés viviendo una relación tóxica o abusiva. Considera buscar apoyo y hablar con alguien de confianza.";
      } else if (totalSi >= 6) {
        mensaje = "Estás probablemente en una relación violenta. No estás sola. Busca ayuda profesional, activa un plan de seguridad y considera usar herramientas como la app Aliada.";
      }

      document.getElementById('result').textContent = `Respuestas SÍ: ${totalSi}. ${mensaje}`;
      // Opcional: desplazar hacia el resultado
      document.getElementById('result').scrollIntoView({behavior: 'smooth'});
    });
  </script>
</body>
</html>
