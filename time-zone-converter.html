  
  <!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>Time Zone Converter</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      background: #eef8ff;
      display: flex;
      justify-content: center;
      align-items: center;
      min-height: 100vh;
      margin: 0;
    }

    .container {
      background: #fff;
      padding: 25px;
      border-radius: 12px;
      box-shadow: 0 4px 12px rgba(0, 123, 255, 0.15);
      max-width: 400px;
      width: 90%;
      text-align: center;
    }

    h2 {
      color: #007bff;
      margin-bottom: 20px;
    }

    input, select {
      width: 100%;
      padding: 10px;
      margin-top: 10px;
      font-size: 16px;
      border-radius: 8px;
      border: 1px solid #ccc;
    }

    button {
      margin-top: 15px;
      padding: 10px 20px;
      background-color: #007bff;
      color: white;
      border: none;
      border-radius: 8px;
      cursor: pointer;
      font-size: 16px;
    }

    button:hover {
      background-color: #0056b3;
    }

    .result {
      margin-top: 20px;
      font-size: 18px;
      font-weight: bold;
      color: #333;
    }
  </style>
</head>
<body>
  <div class="container">
    <h2>Time Zone Converter</h2>

    <label>Select Date & Time</label>
    <input type="datetime-local" id="dateInput" />

    <label>From Time Zone</label>
    <select id="fromZone"></select>

    <label>To Time Zone</label>
    <select id="toZone"></select>

    <button onclick="convertTime()">Convert</button>

    <div class="result" id="outputResult"></div>
  </div>

  <script>
    const timeZones = Intl.supportedValuesOf("timeZone");

    const fromZone = document.getElementById("fromZone");
    const toZone = document.getElementById("toZone");

    timeZones.forEach(zone => {
      const opt1 = document.createElement("option");
      const opt2 = document.createElement("option");
      opt1.value = opt2.value = zone;
      opt1.textContent = opt2.textContent = zone;
      fromZone.appendChild(opt1);
      toZone.appendChild(opt2);
    });

    // Set default to browser time zone
    fromZone.value = Intl.DateTimeFormat().resolvedOptions().timeZone;
    toZone.value = "UTC";

    function convertTime() {
      const dateInput = document.getElementById("dateInput").value;
      const from = fromZone.value;
      const to = toZone.value;
      const resultBox = document.getElementById("outputResult");

      if (!dateInput) {
        resultBox.textContent = "Please select a date and time.";
        return;
      }

      const date = new Date(dateInput);
      const utcDate = new Date(date.toLocaleString("en-US", { timeZone: from }));
      const targetTime = new Date(utcDate.toLocaleString("en-US", { timeZone: to }));

      resultBox.textContent = `Converted Time: ${targetTime.toLocaleString()} (${to})`;
    }
  </script>
</body>
</html>

  
  
