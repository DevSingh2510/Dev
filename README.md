<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Just Curious 😌</title>

<style>
    body {
        background: linear-gradient(135deg, #141e30, #243b55);
        font-family: Arial, sans-serif;
        height: 100vh;
        margin: 0;
        overflow: hidden;
        display: flex;
        justify-content: center;
        align-items: center;
    }

    .card {
        background: white;
        width: 85%;
        max-width: 350px;
        padding: 30px 20px;
        border-radius: 22px;
        text-align: center;
        box-shadow: 0 20px 40px rgba(0,0,0,0.35);
        position: relative;
        z-index: 10;
    }

    h1 {
        color: #243b55;
        font-size: 22px;
        line-height: 1.4;
        margin-bottom: 20px;
    }

    p {
        color: #555;
        font-size: 15px;
        margin-bottom: 30px;
    }

    .buttons {
        position: relative;
        height: 140px;
    }

    button {
        padding: 14px 26px;
        font-size: 18px;
        border-radius: 30px;
        border: none;
        cursor: pointer;
        transition: all 0.25s ease;
    }

    #yes {
        background-color: #243b55;
        color: white;
    }

    #no {
        background-color: #eee;
        color: #999;
        position: absolute;
        left: 50%;
        top: 70px;
        transform: translateX(-50%);
    }
</style>
</head>

<body>

<div class="card">
    <h1>Hey Aishwarya 👀</h1>
    <p>
        Serious question.<br>
        No overthinking allowed 😌
    </p>

    <h1>Can I stalk you?</h1>

    <div class="buttons">
        <button id="yes" onclick="yesClicked()">YES 😏</button>
        <button id="no">NO 🙄</button>
    </div>
</div>

<script>
    const noBtn = document.getElementById("no");

    function moveNo() {
        const x = Math.random() * (window.innerWidth - 120);
        const y = Math.random() * (window.innerHeight - 120);
        noBtn.style.left = x + "px";
        noBtn.style.top = y + "px";
    }

    // Mobile touch
    noBtn.addEventListener("touchstart", moveNo);
    // Desktop fallback
    noBtn.addEventListener("mouseover", moveNo);

    function yesClicked() {
        document.body.innerHTML = `
        <div style="
            height:100vh;
            display:flex;
            justify-content:center;
            align-items:center;
            text-align:center;
            background:linear-gradient(135deg,#000428,#004e92);
            font-family:Arial;
            padding:20px;
            color:white;
        ">
            <h1 style="line-height:1.5;">
                Too late 😈<br><br>
                You tried to say NO,<br>
                but destiny said YES 😌<br><br>
                Stalker mode: ACTIVATED 👀📱
            </h1>
        </div>
        `;
    }
</script>

</body>
</html>
