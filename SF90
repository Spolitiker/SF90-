<!DOCTYPE html>
<html lang="sk">
<head>
  <meta charset="UTF-8" />
  <title>ROBOT CONTROL</title>
  <meta name="viewport" content="width=device-width, initial-scale=1" />

  <style>
    body {
      margin: 0;
      height: 100vh;
      background: radial-gradient(circle at top, #222 0%, #000 70%);
      display: flex;
      justify-content: center;
      align-items: center;
      font-family: 'Arial Black', Arial, sans-serif;
      color: white;
    }

    .panel {
      width: 90%;
      max-width: 420px;
      height: 60%;
      background: linear-gradient(145deg, #111, #1c1c1c);
      border-radius: 30px;
      box-shadow: inset 0 0 30px #000, 0 0 40px rgba(255,0,0,0.2);
      display: flex;
      flex-direction: column;
      justify-content: space-around;
      align-items: center;
      text-align: center;
    }

    .status {
      width: 18px;
      height: 18px;
      border-radius: 50%;
      background: red;
      box-shadow: 0 0 10px red;
      transition: 0.3s;
      margin-bottom: 10px;
    }

    .status.on {
      background: #00ff66;
      box-shadow: 0 0 15px #00ff66;
    }

    button {
      width: 85%;
      height: 35%;
      font-size: 2.2rem;
      font-weight: bold;
      border: none;
      border-radius: 50px;
      color: white;
      background: linear-gradient(180deg, #ff3b3b, #a80000);
      box-shadow: 0 8px 0 #5c0000;
      transition: 0.15s;
      cursor: pointer;
    }

    button.on {
      background: linear-gradient(180deg, #2ecc71, #0f8a3c);
      box-shadow: 0 8px 0 #0b5a28;
    }

    button:active {
      transform: translateY(6px);
      box-shadow: 0 2px 0 #000;
    }

    .label {
      letter-spacing: 2px;
      opacity: 0.8;
      margin: 5px 0;
      user-select: none;
    }
  </style>
</head>

<body>
  <div class="panel">
    <div class="label">ROBOT STATUS</div>
    <div id="statusLed" class="status"></div>

    <button id="robotBtn">ENGINE START</button>

    <div class="label">SF90 CONTROL</div>
  </div>

  <script>
    let robotOn = false;
    const btn = document.getElementById("robotBtn");
    const led = document.getElementById("statusLed");

    btn.addEventListener("click", () => {
      robotOn = !robotOn;

      if (robotOn) {
        btn.textContent = "ENGINE STOP";
        btn.classList.add("on");
        led.classList.add("on");
        sendCommand("on");
      } else {
        btn.textContent = "ENGINE START";
        btn.classList.remove("on");
        led.classList.remove("on");
        sendCommand("off");
      }
    });

    function sendCommand(state) {
      console.log("Robot state:", state);

      // Tu odkomentuj a uprav podľa svojej ESP/server adresy:
      // fetch("http://IP_TVOJHO_ESP/robot?state=" + state)
      //   .then(res => console.log("Príkaz odoslaný"))
      //   .catch(err => console.error("Chyba:", err));
    }
  </script>
</body>
</html>
