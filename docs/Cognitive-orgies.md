<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Nomadic Infrastructure · Theo Jansen Workshop</title>
    <style>
        body {
            font-family: system-ui, -apple-system, 'Segoe UI', sans-serif;
            max-width: 900px;
            margin: 0 auto;
            padding: 40px 20px;
            background: #fafaf7;
            color: #1a1e24;
            line-height: 1.5;
        }
        h1 {
            font-size: 2rem;
            margin-bottom: 0.25rem;
        }
        h2 {
            font-size: 1.5rem;
            margin-top: 2rem;
            margin-bottom: 1rem;
            border-left: 4px solid #2b7a4b;
            padding-left: 1rem;
        }
        h3 {
            font-size: 1.2rem;
            margin-top: 1.5rem;
            margin-bottom: 0.5rem;
            color: #1f5e3a;
        }
        p {
            margin-bottom: 1rem;
            text-align: justify;
        }
        img {
            max-width: 100%;
            height: auto;
            margin: 1rem 0;
            border-radius: 12px;
            background: #eae8e0;
            display: block;
        }
        video {
            max-width: 100%;
            height: auto;
            margin: 1rem 0;
            border-radius: 12px;
            background: #1a1a1a;
            display: block;
        }
        hr {
            margin: 2rem 0;
            border: none;
            height: 1px;
            background: #ccc;
        }
        .question-box {
            background: #eef5ea;
            padding: 1.5rem;
            border-radius: 16px;
            margin: 1rem 0;
            text-align: center;
            font-weight: 500;
        }
    </style>
</head>
<body>

<h1>🚶 Nomadic Infrastructure for Urban Microecosystems</h1>
<p><strong>Antonio García Fernández</strong> · Workshop collaboration with Erandi · Design Studio Course</p>

<hr>

<h2>Context</h2>
<p>In this one-week workshop, we worked as a team to create a prototype that would help us continue researching our field of interest and support the development of our main project for the Design Studio course. I carried out this activity with Erandi, whose research field focuses on studying alternative perspectives within the context of the city, moving away from the anthropocentric view. My field of study is urban mobility, so to create a prototype that would fit both fields, we looked for common points that would help us develop an idea.</p>

<img src="Captura_de_pantalla_2026-02-09_142615.jpg" alt="workshop process">

<h2>Points of Connection</h2>
<p>We ended up finding points of connection in our interests and in relation to our fields of study, specifically in low-tech approaches, decentralization, and urban space. We linked these points to our respective research areas: mobility (mine) and multispecies and non-human perspectives (hers). Based on these connections, we proposed our prototype called <strong>‘Nomadic Infrastructure for Urban Microecosystems’</strong>.</p>

<img src="Captura_de_pantalla_2026-02-09_143012.jpg" alt="concept">

<h2>Research Question</h2>
<div class="question-box">
    <p>How can we create an autonomous mechanical organism, inspired by walking structures, that transports environmental conditions (shade, humidity, and shelter) to enable the survival of insects and other organisms in hostile urban environments?</p>
</div>

<h2>1 · Sketching the initial idea</h2>
<p>Using this question as our guide, we began sketching and shaping the prototype, drawing inspiration from the fascinating mechanisms of Theo Jansen and his kinetic sculptures. The concept consists of creating a machine that searches for the perfect conditions for a microecosystem of its own. It moves because urban hostility is not static. Heat, shade, dryness, and exposure shift constantly in the city and most non-human species lack the ability to escape them. Mobility becomes a survival strategy.</p>
<img src="boceto1.jpg" alt="sketch 1">
<img src="boceto2.jpg" alt="sketch 2">

<h2>2 · Laser cutting the pieces</h2>
<p>To achieve our goal, we needed: a mobile, mechanical, functional, and autonomous structure; a terrarium to hold soil, moss, and other elements to create suitable conditions for microorganisms; and the appropriate electronic components to measure the conditions of that micro-ecosystem. We downloaded the files for the Theo Jansen mechanism for the moving structure and cut them using the laser cutter.</p>
<img src="WhatsApp_Image_2026-02-06_at_14.10.00.jpg" alt="laser cut 1">
<img src="WhatsApp_Image_2026-02-06_at_14.10.00_1.jpg" alt="laser cut 2">

<h2>3 · Assembling the structure</h2>
<p>We assembled the mechanism — 12 legs in total. We had to buy a lot of screws from the hardware store, and it was tricky to tighten the nuts just enough to allow movement without making the structure unstable. We mounted the two servomotors with the legs through a shaft, which would rotate gears when the motors were activated, causing the mechanism to move and the structure to start walking.</p>
<img src="WhatsApp_Image_2026-02-06_at_14.10.00_4.jpg" alt="assembly 1">
<img src="WhatsApp_Image_2026-02-06_at_14.10.01_3.jpg" alt="assembly 2">

<h2>4 · The terrarium & sensors</h2>
<p>With the Arduino, we prepared the most important part of the prototype: 3 sensors in total — one humidity sensor, one photosensitive sensor, and one temperature sensor. This way, we tell the two servo motors when they need to move to search for a more suitable habitat for the organisms in the micro-ecosystem. We designed a terrarium to hold the soil, moss, and worms. We laser-cut it entirely in MDF, and then assembled it together with the structure, Arduino, and batteries.</p>
<img src="WhatsApp_Image_2026-02-06_at_14.10.00_2.jpg" alt="terrarium">
<img src="WhatsApp_Image_2026-02-06_at_14.10.01_4.jpg" alt="sensors">

<h2>5 · Final assembly</h2>
<p>The final step was to assemble the mobile structure with the terrarium, which would interact through the sensors, and the Arduino would activate the servomotors when there was a lack or excess of light, humidity, or temperature.</p>
<img src="WhatsApp_Image_2026-02-06_at_14.25.54.jpg" alt="final 1">
<img src="WhatsApp_Image_2026-02-06_at_14.25.54_1.jpg" alt="final 2">

<hr>

<h2>Result and reflections</h2>

<h3>Final prototype</h3>
<p>The prototype merges low-tech walking principles with responsive ecology: a self-contained terrarium carried by a 12-legged kinetic chassis. Sensors detect critical fluctuations and trigger movement – an attempt to give a micro-ecosystem agency to flee hostile spots. Though still a work in progress, it embodies a shift from static green infrastructure to nomadic, multispecies care. This collaborative prototype opened new intersections between mobility studies and non-human perspectives. We realized that movement can be a form of micro-refuge, and that designing for more-than-human cities demands active, modular, low-energy solutions.</p>
<img src="_jsla04uz6a.jpg" alt="final prototype">

<h3>Circuit diagram</h3>
<p>Looking at the final Arduino circuit diagram, we can see how the sensors, actuators, and microcontroller work together to make the prototype respond to environmental conditions. Ideally, we would have liked to include ultrasonic or proximity sensors so that the prototype could avoid obstacles and be more aware of its surroundings, but we didn't have enough time to implement them. Nevertheless, the current logic (humidity & temp & light) already allows reactive displacement, which represents a fundamental step towards autonomous ecological machines.</p>
<img src="captura_de_pantalla_2026-02-06_144044_sFLHTnbYxC.jpg" alt="circuit diagram">

<h3>The main issue</h3>
<p>The main problem we encountered with the project was the servomotors, which have a 180-degree range, preventing the mechanism from moving in a specific direction and only allowing it to sway slightly back and forth. If it weren't for this issue and a few adjustments needed on the leg shafts, the prototype would have achieved its goal, but we will continue working to make it fully functional. Future iterations will use continuous rotation servos or stepper motors, plus improved crankshaft alignment. However, the conceptual and mechanical foundations are solid: a walking refuge that responds to urban microclimates.</p>
<video src="WhatsApp_Video_2026-02-06_at_15.18.11.mp4" autoplay loop muted playsinline></video>

<hr>

<h3>✨ Reflections</h3>
<p>This project has been a turning point in my way of understanding mobility. Beyond the urban planning charts, traffic flows, and human-centered efficiency metrics, building the Nomadic Infrastructure forced me to get my hands dirty — literally assembling legs, calibrating sensors, and failing with servomotors. It helped me realize that creating complex mechanical structures is not just an engineering challenge but a design speculation tool.</p>

<p>I discovered that mobility does not have to be fast, nor anthropocentric. The slow, fragile, almost clumsy walk of our twelve-legged organism proposed an alternative: movement as survival, not as optimization. This speculative shift opens unexpected territories — what if drones in the future do not deliver packages but carry micro-refuges for pollinators? What if robotic mobility is reimagined as a multispecies choreography rather than logistics?</p>

<p>The workshop allowed me to speculate with robotic mobility for other species, to think of machines that serve ecological thresholds instead of human desires. I am leaving this process with a new sensitivity: designing movement means designing attention, care, and the right to escape hostile ground — whether you are a worm, a beetle, or a future urban drone.</p>

<hr>
<p><strong>Team:</strong> Antonio García Fernández · Erandi<br>
Prototype inspired by Theo Jansen · Arduino · Laser cutting · 3D printing · Silicone mold · Pine resin casting</p>

</body>
</html>