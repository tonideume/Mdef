
# Extended Intelligence II

<!DOCTYPE html>
<html>
<head>
<style>
.bloque {
    display: flex;
    gap: 20px;
    margin-bottom: 80px; /* ← ESPACIO ABAJO */
}
.bloque {
    display: flex;
    gap: 20px;
}
.bloque-texto {
    width: 50%;
      text-align: justify;
}
.bloque-imagen {
    width: 40%;
}
.bloque-imagen img {
    width: 100%;
}

</style>
</head>
<div class="bloque">
    <div class="bloque-texto">
        <p>
       For this course, we were tasked with developing a concept that incorporated AI, specifically AI agents, ideally using them as a bridge between humans and technology.

We decided to focus on a music-related idea. Initially, we wanted to create an object that would allow users to jam with just their fingers, exploring the musical world while receiving real-time feedback from an AI agent. The AI would indicate mistakes, suggest improvements, and guide users on how to adjust their playing. However, we quickly realized that this approach was unfeasible due to the project’s time constraints (only two days) and technological limitations—current AI agents are too slow to provide instant responses to users’ movements in a seamless way. Despite this, we wanted to keep the essence of the musical jamming idea and simplify it.

The revised concept allowed users to create rhythms by tapping on a sequence of touch sensors. The AI agent would then analyze the pattern and suggest a song with a similar rhythmic structure, providing a YouTube link for the user to explore.
        </p>
    </div>

 <div class="bloque-imagen">
        <img src="images/WhatsApp Image 2026-02-08 at 18.43.41 (1).jpeg">
    </div>
</div>


Materials used: Raspberry Pi, PC with Arduino, custom-made touch sensor, breadboard, AI agents

The first step was to connect a touch sensor to the Raspberry Pi so we could send touch data to the AI agents. Since we didn’t have a ready-made sensor available, we built a simple one by attaching a thin copper sheet to the breadboard, using its conductivity to detect touch input.

After that, we started working on the code to ensure that the agent would respond correctly to the touch signals. However, this is where we began to encounter several technical issues.

We had very limited time to make the system fully functional, and despite our efforts — and the support from the teacher — we couldn’t manage to achieve the result we were aiming for. Even so, we still wanted to create a representation of how the system would work if we had successfully connected the physical inputs with the digital AI agents, so we focused on defining and organizing the agent workflow.

The concept structure works as follows: once the experience starts, the user touches the sensor. When the touch is detected, the ‘Song AI Agent’ searches online for a track with a rhythm pattern similar to the one created by the user and then suggests it. A second agent generates lyrics based on a color selected by the user. After this, the cycle ends, although the experience can be repeated as many times as the user wants.

# Extended Intelligence II

I would really like to continue learning about AI on my own, deepening my understanding of how it works and how it can be applied in creative and technological projects. I plan to take every opportunity I can to learn more about it, such as workshops, courses, or practical experiences, like the AI workshop that will take place at Elisava next week.


