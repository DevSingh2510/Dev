<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Just Asking 😌</title>

<style>
    body {
        background: linear-gradient(135deg, #1d2671, #c33764);
        font-family: Arial, sans-serif;
        height: 100vh;
        margin: 0;
        display: flex;
        justify-content: center;
        align-items: center;
        overflow: hidden;
    }

    .card {
        background: white;
        width: 85%;
        max-width: 350px;
        padding: 30px 20px;
        border-radius: 20px;
        text-align: center;
        box-shadow: 0 20px 40px rgba(0,0,0,0.3);
    }

    h1 {
        color: #c33764;
        font-size: 22px;
        line-height: 1.4;
        margin-bottom: 25px;
    }

    p {
        color: #444;
        font-size: 15px;
        margin-bottom: 30px;
    }

    .buttons {
        display: flex;
        justify-content: space-around;
        gap: 15px;
    }

    button {
        padding: 14px 24px;
        font-size: 18px;
        border-radius: 30px;
        border: none;
        cursor: pointer;
        width: 120px;
    }

    #yes {
        background-color: #c33764;
        color: white;
    }

    #no {
        background-color: #eee;
        color: #aaa;
        pointer-events: none; /* 😈 NO is disabled */
    }
</style>
</head>

<body>

<div class="card">
    <h1>Hey Aishwarya 👀</h1>
    <p>
        Important question…<br>
        Please think carefully 😌
    </p>

    <h1>Can I stalk you?</h1>

    <div class="buttons">
        <button id="yes" onclick="yesClicked()">YES 😏</button>
        <button id="no">NO 🙄</button>
    </div>
</div>

<script>
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
                Permission granted automatically ✅<br><br>
                FBI mode: ON 👀📱
            </h1>
        </div>
        `;
    }
</script>

</body>
</html>
