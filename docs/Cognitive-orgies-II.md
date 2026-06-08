<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Echo of Mind · Documentation</title>
    <style>
        body {
            font-family: system-ui, -apple-system, 'Segoe UI', sans-serif;
            max-width: 900px;
            margin: 0 auto;
            padding: 40px 20px;
            background: #0a0a0f;
            color: #e0e0e0;
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
            border-left: 4px solid #7c3aed;
            padding-left: 1rem;
        }
        h3 {
            font-size: 1.2rem;
            margin-top: 1.5rem;
            margin-bottom: 0.5rem;
            color: #c4b5fd;
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
            background: #1a1a2a;
            display: block;
        }
        hr {
            margin: 2rem 0;
            border: none;
            height: 1px;
            background: #2a2a3a;
        }
        .card {
            background: #12121a;
            padding: 1rem;
            border-radius: 16px;
            margin: 1rem 0;
            border: 1px solid #2a2a3a;
        }
        a {
            color: #a78bfa;
        }
    </style>
</head>
<body>

<h1>🧠 Echo of Mind</h1>
<p><strong>Antonio García Fernández</strong> · Team: Hannah Peevey, alerivera · Created March 6, 2026</p>

<hr>

<h2>Logic & Theoretical Grounding</h2>

<p><strong>1. Intelligence Definitions</strong><br>
We are operating on the premise that intelligence is an entity that acts upon its environment according to its own logic. We are categorizing "Hallucinations" not as errors, but as stimulus-independent percepts. The Goal: To create a "Bridge, Not a Barrier", an intuitive interface that feels natural rather than intimidating.</p>

<p><strong>2. Communication & "Dreaming"</strong><br>
We define the interaction as a category of perceptual experiences created entirely by the brain (or AI) without external sensory input. The Mechanism: Stimulus-Independent Perceptions (SIPs). The Output: Exploring the "Intelligence" way of communicating dreams through voice (input) and sensory simulation (output).</p>

<p><strong>3. The Layered Hierarchy</strong><br>
Biological: Dreams, hallucinations, and the subconscious.<br>
Technological: The "Bridge"—the glitch mechanism and triggers.<br>
Collective Archive: The final website/storage of the shared experience.</p>

<h2>Day 1: System Infrastructure</h2>
<p><strong>Daily Goals:</strong> Hardware Backbone: Power and network the Raspberry Pi 5. Remote Access: Establish SSH pipeline for headless development. Housing: Design and 3D print the first iteration of the device chassis.</p>
<p><strong>Tasks Completed:</strong> Connected Raspberry Pi 5 to a dedicated screen and independent power source. Configured Pi 5 to run on a mobile hotspot with full internet access. Successfully established SSH communication from laptop to Pi 5. Modified the 3D model to fit the device screen and completed the 3D print. Defined the split-intelligence system (Collective vs. Personal).</p>
<p><strong>Errors & Roadblocks:</strong> GitHub Access: Failed to clone the repository. Account Integration: Difficulty linking the Luma account. API Validation: OpenAI API connection errors during initial testing.</p>
<p><strong>Components Used:</strong> Raspberry Pi 5, Integrated Screen, Custom 3D Printed Chassis, OpenAI, Luma, GitHub.</p>

<h2>Day 2: Agent Persona & API Integration</h2>
<p><strong>Daily Goals:</strong> Character Design: Define specific operational "Specs" and personalities for the AI Assistants. Connectivity: Bridge Raspberry Pi 5 with Hugging Face & OpenAI. Multimodal Testing: Successfully trigger image generation via voice command.</p>
<p><strong>Tasks Completed:</strong> Developed detailed Spec Sheets for the AI Assistant. Built specific User Profiles for the device. Successfully established tripartite connection between Hugging Face, OpenAI Assistant, and the Raspberry Pi 5. Successfully generated images based on Voice Input triggers within local development environment.</p>
<p><strong>Errors & Roadblocks:</strong> Pattern Recognition Failure: System failing to detect generated images as coherent "pattern". Deployment Gap: Generative script running on Local Host (laptop), not yet migrated to Raspberry Pi 5.</p>

<h2>Day 3: Physical Refinement & Collective Sync</h2>
<p><strong>Daily Goals:</strong> Aesthetic Control: Fine-tune generative AI output to match visual language. Hardware Ergonomics: Perfect physical housing and tactile interface. Data Loop: Establish bridge between device and web-based Collective Archive with Cloudflare link updating every 4 seconds.</p>
<p><strong>Tasks Completed:</strong> Successfully manipulated AI script to control image style triggered by voice. Iterated heavily on 3D-printed device holder; refined, remodeled, and reprinted chassis. Integrated physical button commands and LED lights via Pico for manual override. Built Collective Archive website and established local server connection syncing device outputs to web interface in real-time.</p>

<hr>

<h2>📟 DEVICE DOCUMENTATION</h2>
![](images/final_device_1.jpg)
<img src="final_device_2.jpg" alt="final device 2">
<img src="final_device_3.jpg" alt="final device 3">

<h2>🔁 SYSTEM ARCHITECTURE SIGNAL FLOW</h2>
<img src="system_architecture.jpg" alt="System Architecture Signal Flow">

<h2>🌙 DOCUMENTED DREAMS</h2>
<img src="dream_1.jpg" alt="dream 1">
<img src="dream_2.jpg" alt="dream 2">
<img src="dream_3.jpg" alt="dream 3">
<img src="dream_4.jpg" alt="dream 4">
<img src="dream_5.jpg" alt="dream 5">
<img src="dream_6.jpg" alt="dream 6">

<h2>📡 COLLECTIVE ARCHIVE</h2>
<p><strong>ACCESS HERE →</strong> <a href="https://hannahpeevey254.github.io/ECHO-OF-MIND/" target="_blank">https://hannahpeevey254.github.io/ECHO-OF-MIND/</a></p>

<h2>🧩 COGNITIVE CONTRIBUTION LABEL</h2>
<img src="cognitive_label.jpg" alt="Cognitive Contribution Label">

<h2>🖼️ FRAME AND STRUCTURE</h2>
<img src="frame_1.jpg" alt="frame 1">
<img src="frame_2.jpg" alt="frame 2">
<img src="frame_3.jpg" alt="frame 3">
<img src="frame_4.jpg" alt="frame 4">
<img src="frame_5.jpg" alt="frame 5">
<img src="frame_6.jpg" alt="frame 5">

<p>For this assignment, we designed and built a structural system intended to house the electronic components of an image-generation AI setup. The device integrated an Arduino and a Raspberry Pi, which were used to control and run the generative system.</p>

<p>The project consisted of two main parts. The first part was an organic structural element that elevated and supported the entire device. This structure was modeled in Blender, where we explored more fluid and expressive forms that contrasted with the technical nature of the electronics. The second part was a protective casing designed in Rhino, which contained the electronic components such as the Arduino and the Raspberry Pi. This casing was designed to be more functional and precise, focusing on the organization and protection of the hardware.</p>

<p>During the development of the project, we encountered several issues related to the physical balance of the device. One of the main problems was that we did not correctly calculate the center of gravity of the electronic components inside the casing. As a result, the structural support was not properly designed to compensate for the weight distribution.</p>

<p>When the two parts were finally assembled, the device tended to tilt forward because most of the weight was concentrated in the front section of the casing. This meant that the structure could not stand upright on its own and had to be held or supported to prevent it from falling forward. Although this problem revealed a flaw in the design process, it also highlighted the importance of considering weight distribution and balance when designing structures that integrate electronic hardware.</p>

<h2>📐 Circuit Diagram</h2>
<img src="circuit_diagram.jpg" alt="Circuit Diagram">

<h2>🖨️ 3D Model</h2>
<p>We designed and built a shell for the device using Rhino and Blender - to then 3D print these models.</p>

<h2>💻 Code</h2>
<p>Python scripts for OpenAI Assistant integration, Hugging Face inference, Flask local server, and image style manipulation. Full repository available upon request.</p>

<hr>

<h2>✨ Reflections on Generative AI</h2>
<p>This project has radically transformed my understanding of generative AI. Before Echo of Mind, I saw AI image generation as a tool for producing visuals on demand — a faster, more efficient rendering engine. But working hands-on with the hallucinations, the stimulus-independent percepts, and the fragile bridge between voice and generated dreamscapes taught me something deeper.</p>

<p>I learned that generative AI is not just a production machine; it is a mirror of latent cognition. When the system failed to recognize image patterns, or when it produced images that drifted away from my prompts, I realized that those "errors" were actually the most interesting part — the AI dreaming in its own language. The glitch became the message.</p>

<p>Building the split-intelligence architecture (personal agent vs. collective archive) forced me to confront questions I had never asked: What does an AI remember? How does it hallucinate? Can a machine have a subconscious? By designing the spec sheets, user profiles, and the 4-second sync loop to the archive, I understood that generative AI is fundamentally a collaborative speculative practice. It is not about controlling the output, but about orchestrating a conversation between human intention and machine serendipity.</p>

<p>Today, I no longer see generative models as simple tools. I see them as co-creators with their own kind of logic, failure modes, and aesthetic preferences. Echo of Mind taught me to embrace the unpredictable, to design for emergence, and to listen to what the machine dreams — because sometimes the most powerful images are the ones neither side expected.</p>

<hr>
<p><strong>Team Echo of Mind:</strong> Hannah Peevey · alerivera · Antonio García Fernández<br>
Prototype built on Raspberry Pi 5 · OpenAI · Hugging Face · Flask · Collective Archive live sync</p>

</body>
</html>