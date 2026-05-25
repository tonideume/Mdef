<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Nomadic Infrastructure · Cognitive Orgies Workshop</title>
    <style>
        /* RESET Y ESTILOS GLOBALES */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        body {
            background: #eef2f0;
            font-family: system-ui, -apple-system, 'Segoe UI', Roboto, 'Helvetica Neue', sans-serif;
            line-height: 1.5;
            color: #1a2a1f;
            padding: 40px 20px;
        }
 /* CONTENEDOR PRINCIPAL: ANCHO MÁXIMO LEGIBLE */
        .main-container {
            max-width: 1200px;
            margin: 0 auto;
            background: white;
            border-radius: 32px;
            box-shadow: 0 20px 35px -12px rgba(0, 0, 0, 0.1);
            padding: 40px 48px;
        }
 /* RESPONSIVE */
        @media (max-width: 800px) {
            body {
                padding: 20px 12px;
            }
            .main-container {
                padding: 24px 20px;
            }
        }
 /* TÍTULOS */
        .section-title {
            font-size: 28px;
            font-weight: 700;
            margin: 40px 0 20px 0;
            padding-left: 16px;
            border-left: 6px solid #2c7a4b;
            color: #1e3a2f;
        }
        .subtitle-highlight {
            font-size: 22px;
            font-weight: 700;
            color: #1f6e43;
            display: inline-block;
            margin-bottom: 12px;
        }
        /* BLOQUE FLEX: TEXTO + IMAGEN (50% - 50%) */
        .flex-block {
            display: flex;
            flex-wrap: wrap;
            gap: 40px;
            margin-bottom: 50px;
            align-items: center;
        }
        .flex-text {
            flex: 1;
            min-width: 250px;
            text-align: justify;
        }
        .flex-media {
            flex: 1;
            min-width: 250px;
        }
        .flex-media img, .flex-media video {
            width: 100%;
            border-radius: 24px;
            box-shadow: 0 8px 20px rgba(0, 0, 0, 0.08);
            display: block;
            background: #e9e9df;
        }
        /* orden invertido */
        .reverse {
            flex-direction: row-reverse;
        }
 /* DOBLE COLUMNA DE TEXTO */
        .double-col {
            display: flex;
            flex-wrap: wrap;
            gap: 40px;
            margin: 30px 0 30px 0;
        }
        .double-col > div {
            flex: 1;
            text-align: justify;
            font-size: 1rem;
        }
/* BLOQUE DE TRES COLUMNAS (texto + dos imágenes) */
        .triple-row {
            display: flex;
            flex-wrap: wrap;
            gap: 30px;
            margin: 45px 0 55px 0;
        }
        .triple-text {
            flex: 1.2;
            min-width: 220px;
            text-align: justify;
        }
        .triple-img {
            flex: 1;
            min-width: 180px;
        }
        .triple-img img {
            width: 100%;
            height: 260px;
            object-fit: cover;
            border-radius: 20px;
            background: #dadacf;
            box-shadow: 0 6px 12px rgba(0,0,0,0.05);
        }
        @media (max-width: 780px) {
            .triple-img img {
                height: auto;
                max-height: 250px;
            }
        }
/* PREGUNTA DESTACADA */
        .question-card {
            background: #eef5ea;
            padding: 28px 32px;
            border-radius: 32px;
            margin: 20px 0 30px 0;
            text-align: center;
        }
        .question-card p {
            font-size: 24px;
            font-weight: 500;
            line-height: 1.3;
            color: #1a472a;
        }
/* VIDEO WRAPPER */
        .video-wrapper {
            border-radius: 24px;
            overflow: hidden;
            background: #000;
        }
        .video-wrapper video {
            width: 100%;
            display: block;
        }
        hr {
            margin: 40px 0 20px;
            border: none;
            height: 1px;
            background: linear-gradient(to right, #ccc, transparent);
        }
        .caption {
            font-size: 13px;
            text-align: center;
            color: #5f6c5b;
            margin-top: 10px;
        }
    </style>
</head>
<body>
<div class="main-container">
<!-- 1. TEXTO INTRO + IMAGEN (primer bloque) -->
    <div class="flex-block">
        <div class="flex-text">
            <p><strong class="subtitle-highlight">🌀 Cognitive Orgies · workshop week</strong></p>
            <p>In this one-week workshop, we worked as a team to create a prototype that would help us continue researching our field of interest and support the development of our main project for the Design Studio course. I carried out this activity with Erandi, whose research field focuses on studying alternative perspectives within the context of the city, moving away from the anthropocentric view. My field of study is urban mobility, so to create a prototype that would fit both fields, we looked for common points that would help us develop an idea.</p>
        </div>
        <div class="flex-media">
            <!-- REEMPLAZA image1.jpg por tu imagen real -->
            <img src="images/Captura de pantalla 2026-02-09 142615.png" alt="workshop process">
        </div>
    </div>
<!-- DOBLE TEXTO (conexión de intereses) -->
    <div class="double-col">
        <div>We ended up finding points of connection in our interests and in relation to our fields of study, specifically in low-tech approaches, decentralization, and urban space. We linked these points to our respective research areas: mobility (mine) and multispecies and</div>
        <div>non-human perspectives (hers). Based on these connections, we proposed our prototype called <strong>‘Nomadic Infrastructure for Urban Microecosystems’</strong>.</div>
    </div>
 <!-- IMAGEN CENTRAL (ancho completo) -->
    <div style="margin: 20px 0 35px;">
        <img src="images/Captura de pantalla 2026-02-09 143012.png" alt="concept overview" style="width:100%; border-radius: 28px; box-shadow: 0 6px 14px rgba(0,0,0,0.05);">
    </div>
 <!-- RESEARCH QUESTION -->
    <div class="section-title">📡 Research Question</div>
    <div class="question-card">
        <p>How can we create an autonomous mechanical organism, inspired by walking structures, that transports environmental conditions (shade, humidity, and shelter) to enable the survival of insects and other organisms in hostile urban environments?</p>
    </div>
 <!-- 1 - Sketching -->
    <div class="triple-row">
        <div class="triple-text">
            <span class="subtitle-highlight">1 · Sketching the initial idea</span>
            <p>Using this question as our guide, we began sketching and shaping the prototype, drawing inspiration from the fascinating mechanisms of Theo Jansen and his kinetic sculptures. The concept consists of creating a machine that searches the perfect conditions for a microecosystem of its own. It moves because urban hostility is not static. Heat, shade, dryness, and exposure shift constantly in the city and most non-human species lack the ability to escape them. Mobility becomes a survival strategy.</p>
        </div>
        <div class="triple-img"><img src="images/boceto1.png" alt="sketch 1"><div class="caption">walking sketches</div></div>
        <div class="triple-img"><img src="images/boceto2.png" alt="sketch 2"><div class="caption">kinetic mechanism</div></div>
    </div>
<!-- 2 - Laser cutting -->
    <div class="triple-row">
        <div class="triple-text">
            <span class="subtitle-highlight">2 · Laser cutting the pieces</span>
            <p>To achieve our goal, we needed: a mobile, mechanical, functional, and autonomous structure; a terrarium to hold soil, moss, and other elements to create suitable conditions for microorganisms; and the appropriate electronic components to measure the conditions of that micro-ecosystem. We downloaded the files for the Theo Jansen mechanism for the moving structure and cut them using the laser cutter.</p>
        </div>
        <div class="triple-img"><img src="images/WhatsApp Image 2026-02-06 at 14.10.00.jpeg" alt="laser cut pieces"></div>
        <div class="triple-img"><img src="images/WhatsApp Image 2026-02-06 at 14.10.00 (1).jpeg" alt="mdf parts"></div>
    </div>
 <!-- 3 - Assembling -->
    <div class="triple-row">
        <div class="triple-text">
            <span class="subtitle-highlight">3 · Assembling the structure</span>
            <p>We assembled the mechanism — 12 legs in total. We had to buy a lot of screws from the hardware store, and it was tricky to tighten the nuts just enough to allow movement without making the structure unstable. We mounted the two servomotors with the legs through a shaft, which would rotate gears when the motors were activated, causing the mechanism to move and the structure to start walking.</p>
        </div>
        <div class="triple-img"><img src="images/WhatsApp Image 2026-02-06 at 14.10.00 (4).jpeg" alt="leg assembly"></div>
        <div class="triple-img"><img src="images/WhatsApp Image 2026-02-06 at 14.10.01 (3).jpeg" alt="servo mount"></div>
    </div>
<!-- 4 - Terrarium & sensors -->
    <div class="triple-row">
        <div class="triple-text">
            <span class="subtitle-highlight">4 · The terrarium & sensors</span>
            <p>With the Arduino, we prepared the most important part of the prototype: 3 sensors in total — one humidity sensor, one photosensitive sensor, and one temperature sensor. This way, we tell the two servo motors when they need to move to search for a more suitable habitat for the organisms in the micro-ecosystem. We designed a terrarium to hold the soil, moss, and worms. We laser-cut it entirely in MDF, and then assembled it together with the structure, Arduino, and batteries.</p>
        </div>
        <div class="triple-img"><img src="images/WhatsApp Image 2026-02-06 at 14.10.00 (2).jpeg" alt="terrarium design"></div>
        <div class="triple-img"><img src="images/WhatsApp Image 2026-02-06 at 14.10.01 (4).jpeg" alt="sensor wiring"></div>
    </div>
<!-- 5 - Final step -->
    <div class="triple-row">
        <div class="triple-text">
            <span class="subtitle-highlight">5 · Final assembly</span>
            <p>The final step was to assemble the mobile structure with the terrarium, which would interact through the sensors, and the Arduino would activate the servomotors when there was a lack or excess of light, humidity, or temperature.</p>
        </div>
        <div class="triple-img"><img src="images/WhatsApp Image 2026-02-06 at 14.25.54.jpeg" alt="final prototype 1"></div>
        <div class="triple-img"><img src="images/WhatsApp Image 2026-02-06 at 14.25.54 (1).jpeg" alt="final prototype 2"></div>
    </div>
 <!-- RESULTADOS -->
    <div class="section-title">📌 Final result </div>
<!-- Final prototype (texto + imagen) -->
    <div class="flex-block">
        <div class="flex-text">
            <span class="subtitle-highlight">Final prototype</span>
            <p>The prototype merges low-tech walking principles with responsive ecology: a self-contained terrarium carried by a 12-legged kinetic chassis. Sensors detect critical fluctuations and trigger movement – an attempt to give a micro-ecosystem agency to flee hostile spots. Though still a work in progress, it embodies a shift from static green infrastructure to nomadic, multispecies care.</p>
            <p>This collaborative prototype opened new intersections between mobility studies and non-human perspectives. We realized that movement can be a form of micro-refuge.</p>
        </div>
        <div class="flex-media">
            <img src="images/_jsla04uz6a.avif" alt="full prototype">
        </div>
    </div>
 <!-- Circuit diagram -->
    <div class="flex-block reverse">
        <div class="flex-text">
            <span class="subtitle-highlight">Circuit diagram</span>
            <p>Looking at the final Arduino circuit diagram, we can see how the sensors, actuators, and microcontroller work together to make the prototype respond to environmental conditions. Ideally, we would have liked to include ultrasonic or proximity sensors so that the prototype could avoid obstacles and be more aware of its surroundings, but we didn’t have enough time to implement them.</p>
            <p>Nevertheless, the current logic (humidity & temp & light) already allows reactive displacement, which represents a fundamental step towards autonomous ecological machines.</p>
        </div>
        <div class="flex-media">
            <img src="images/captura_de_pantalla_2026-02-06_144044_sFLHTnbYxC.avif" alt="circuit diagram">
        </div>
    </div>
<!-- Main issue + VIDEO -->
    <div class="flex-block">
        <div class="flex-text">
            <span class="subtitle-highlight">⚙️ The main issue</span>
            <p>The main problem we encountered with the project was the servomotors, which have a 180-degree range, preventing the mechanism from moving in a specific direction and only allowing it to sway slightly back and forth. If it weren't for this issue and a few adjustments needed on the leg shafts, the prototype would have achieved its goal, but we will continue working to make it fully functional.</p>
            <p>Future iterations will use continuous rotation servos or stepper motors, plus improved crankshaft alignment. However, the conceptual and mechanical foundations are solid.</p>
        </div>
        <div class="flex-media">
            <div class="video-wrapper">
                <video src="images/WhatsApp Video 2026-02-06 at 15.18.11.mp4" autoplay loop muted playsinline></video>
            </div>
            <div class="caption">Prototype test: limited motion due to 180° servo range</div>
        </div>
    </div>
    <!-- ========== REFLECTIONS FINAL SECTION ========== -->
<div class="section-title" style="margin-top: 60px;">✨ Reflections</div>

<div style="background: linear-gradient(135deg, #f0f4eb 0%, #e6ede0 100%); border-radius: 28px; padding: 2.2rem 2rem; margin: 20px 0 30px 0; box-shadow: 0 8px 18px rgba(0,0,0,0.05);">
    <p style="font-size: 1.08rem; line-height: 1.6; margin-bottom: 1.4rem; text-align: justify;">
        This project has been a turning point in my way of understanding mobility. Beyond the urban planning charts, traffic flows, and human-centered efficiency metrics, building the <strong>Nomadic Infrastructure</strong> forced me to get my hands dirty — literally assembling legs, calibrating sensors, and failing with servomotors. It helped me realize that <strong>creating complex mechanical structures</strong> is not just an engineering challenge but a design speculation tool.
    </p>
    <p style="font-size: 1.08rem; line-height: 1.6; margin-bottom: 1.4rem; text-align: justify;">
        I discovered that <strong>mobility does not have to be fast, nor anthropocentric</strong>. The slow, fragile, almost clumsy walk of our twelve-legged organism proposed an alternative: movement as survival, not as optimization. This speculative shift opens unexpected territories — what if drones in the future do not deliver packages but carry micro-refuges for pollinators? What if robotic mobility is reimagined as a multispecies choreography rather than logistics?
    </p>
    <p style="font-size: 1.08rem; line-height: 1.6; margin-bottom: 0; text-align: justify;">
        The workshop allowed me to <strong>speculate with robotic mobility for other species</strong>, to think of machines that serve ecological thresholds instead of human desires. I am leaving this process with a new sensitivity: designing movement means designing attention, care, and the right to escape hostile ground — whether you are a worm, a beetle, or a future urban drone.
    </p>
</div>
    <hr>
    <div style="background: #F5F6F0; border-radius: 24px; padding: 28px; margin-top: 20px;">
        <p style="text-align: center; font-style: italic; font-size: 1rem;">“Nomadic Infrastructure for Urban Microecosystems” questions the static nature of green design. By merging Theo Jansen’s walking creatures with real-time environmental sensing, we propose that future urban refuges might <strong>walk, adapt and search for survival</strong> — a small but radical shift beyond anthropocentric cities.</p>
    </div>

</div> <!-- cierre main-container -->
</body>
</html>