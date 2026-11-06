
<!DOCTYPE html>
<html lang="es">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Muchos TQM 💗</title>

<style>
* {
    box-sizing: border-box;
}

body {
    margin: 0;
    min-height: 100vh;
    font-family: "Trebuchet MS", sans-serif;
    background: linear-gradient(135deg, #ffe0ed, #fff0f6, #f9d9ff);
    display: flex;
    justify-content: center;
    align-items: center;
    overflow-x: hidden;
    color: #a83268;
    text-align: center;
    padding: 25px 12px;
}

.corazones {
    position: fixed;
    inset: 0;
    pointer-events: none;
    overflow: hidden;
}

.corazon {
    position: absolute;
    bottom: -50px;
    font-size: 25px;
    animation: subir 8s linear infinite;
    opacity: 0.7;
}

.corazon:nth-child(1) { left: 8%; animation-delay: 0s; }
.corazon:nth-child(2) { left: 25%; animation-delay: 2s; }
.corazon:nth-child(3) { left: 48%; animation-delay: 4s; }
.corazon:nth-child(4) { left: 70%; animation-delay: 1s; }
.corazon:nth-child(5) { left: 90%; animation-delay: 3s; }

@keyframes subir {
    from { transform: translateY(0) rotate(0deg); }
    to { transform: translateY(-110vh) rotate(360deg); }
}

.tarjeta {
    position: relative;
    width: min(100%, 470px);
    background: rgba(255, 255, 255, 0.88);
    border: 3px solid #ffc1dc;
    border-radius: 30px;
    padding: 30px 20px;
    box-shadow: 0 12px 35px #e99abb66;
    animation: aparecer 1s ease;
}

@keyframes aparecer {
    from { opacity: 0; transform: translateY(25px); }
    to { opacity: 1; transform: translateY(0); }
}

h1 {
    font-size: clamp(28px, 7vw, 38px);
    margin: 8px 0;
    color: #e34d91;
}

.gatitos {
    font-size: clamp(65px, 17vw, 90px);
    margin: 12px 0;
    animation: saltito 2s infinite ease-in-out;
}

@keyframes saltito {
    0%, 100% { transform: translateY(0); }
    50% { transform: translateY(-9px); }
}

.mensaje {
    font-size: 18px;
    line-height: 1.7;
}

.tqm {
    display: flex;
    justify-content: center;
    flex-wrap: wrap;
    gap: 8px;
    margin: 20px 0;
}

.tqm span {
    background: #ffe1ef;
    border: 1px solid #ffb4d5;
    border-radius: 20px;
    padding: 7px 12px;
    animation: latido 1.5s infinite;
}

@keyframes latido {
    0%, 100% { transform: scale(1); }
    50% { transform: scale(1.07); }
}

button {
    border: none;
    background: #f062a0;
    color: white;
    padding: 13px 22px;
    border-radius: 25px;
    font-size: 16px;
    font-weight: bold;
    cursor: pointer;
    box-shadow: 0 5px 12px #e78ab866;
}

button:hover {
    background: #d94385;
    transform: scale(1.04);
}

#sorpresa {
    display: none;
    margin-top: 20px;
    padding: 15px;
    background: #fff0f7;
    border-radius: 18px;
    font-size: 19px;
    line-height: 1.6;
}

footer {
    margin-top: 22px;
    font-size: 13px;
    color: #bd6590;
}
</style>
</head>

<body>

<div class="corazones">
    <div class="corazon">💗</div>
    <div class="corazon">💕</div>
    <div class="corazon">💖</div>
    <div class="corazon">💘</div>
    <div class="corazon">💞</div>
</div>

<main class="tarjeta">

    <div>🎀 💌 🎀</div>

    <h1>Muchos TQM 💗</h1>

    <div class="gatitos">🐱💕🐱</div>

    <p class="mensaje">
        Si pudiera enviarte un gatito,<br>
        te mandaría mil para recordarte<br>
        lo mucho que te quiero. 💘💝💓
    </p>

    <div class="tqm">
        <span>TQM 💗</span>
        <span>TQM 💕</span>
        <span>TQM 💘</span>
        <span>TQM 💞</span>
        <span>TQM 💓</span>
        <span>TQM 💝</span>
        <span>TQM 🐱</span>
        <span>TQM 🌷</span>
        <span>TQM ✨</span>
        <span>TQM 💘💝💓</span>
    </div>

    <p class="mensaje">
        Eres mi notificación favorita. 💌<br>
        Mi dosis diaria de felicidad<br>
        y una de las personas que me motiva a ser mejor y con que con sus mensajes me hacen sonreirle al celular. 🐾
    </p>

    <button onclick="mostrarSorpresa()">
        Abrir mi sorpresita 💌
    </button>

    <div id="sorpresa">
        🐱💗 ¡MIAUUU! 💗🐱<br><br>
        Este gatito viene a recordarte<br>
        que mereces muchos abrazos,<br>
        sonrisas y cosas bonitas como yo.<br><br>
        TQM TQM TQM TQM TQM<br>
        💖💕💗💞💘💝💓
    </div>

    <footer>
        Hecho con mucho cariño y patitas de gatito 🐾
    </footer>

</main>

<script>
function mostrarSorpresa() {
    const sorpresa = document.getElementById("sorpresa");

    if (sorpresa.style.display === "block") {
        sorpresa.style.display = "none";
    } else {
        sorpresa.style.display = "block";
    }
}
</script>

</body>
</html>
