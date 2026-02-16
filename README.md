<button class="confetti-button animate__animated animate__bounceIn animate__delay-4s" onclick="launchConfetti()">
    ¡Haz clic aquí para un sorpresa!
</button>

<style>
    .confetti-button {
        background-color: #ffc107; /* Un color dorado/amarillo */
        color: #333;
        border: none;
        padding: 12px 25px;
        border-radius: 30px;
        font-size: 1.1rem;
        cursor: pointer;
        margin-top: 2rem;
        box-shadow: 0 5px 20px rgba(0,0,0,0.1);
        transition: transform 0.2s ease;
    }
    .confetti-button:hover {
        transform: scale(1.05);
    }
</style>

<script src="https://cdn.jsdelivr.net/npm/canvas-confetti@1.5.1/dist/confetti.browser.min.js"></script>
<script>
    function launchConfetti() {
        confetti({
            particleCount: 200,
            spread: 90,
            origin: { y: 0.6 },
            colors: ['#e91e63', '#ffc107', '#ffffff', '#fad0c4']
        });
    }
</script>
