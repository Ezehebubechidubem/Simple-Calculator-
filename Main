<!DOCTYPE html>
<html>
<head>
  <title>Simple Calculator</title>
  <style>
    body {
      display: flex;
      justify-content: center;
      align-items: center;
      height: 100vh;
      background: #f4f4f4;
    }
    .calculator {
      background: #fff;
      padding: 20px;
      border-radius: 10px;
      box-shadow: 0px 0px 10px gray;
    }
    input {
      width: 100%;
      height: 40px;
      margin-bottom: 10px;
      text-align: right;
      font-size: 20px;
      padding: 5px;
    }
    button {
      width: 50px;
      height: 50px;
      margin: 5px;
      font-size: 18px;
    }
  </style>
</head>
<body>

<div class="calculator">
  <input type="text" id="display" readonly>
  <br>
  <button onclick="press('1')">1</button>
  <button onclick="press('2')">2</button>
  <button onclick="press('3')">3</button>
  <button onclick="press('+')">+</button>
  <br>
  <button onclick="press('4')">4</button>
  <button onclick="press('5')">5</button>
  <button onclick="press('6')">6</button>
  <button onclick="press('-')">-</button>
  <br>
  <button onclick="press('7')">7</button>
  <button onclick="press('8')">8</button>
  <button onclick="press('9')">9</button>
  <button onclick="press('*')">*</button>
  <br>
  <button onclick="press('0')">0</button>
  <button onclick="press('/')">/</button>
  <button onclick="calculate()">=</button>
  <button onclick="clearDisplay()">C</button>
</div>

<script>
  function press(value) {
    document.getElementById("display").value += value;
  }

  function calculate() {
    let expression = document.getElementById("display").value;

    // Using if-else to check operator
    if (expression.includes("+")) {
      let parts = expression.split("+");
      document.getElementById("display").value = Number(parts[0]) + Number(parts[1]);
    } 
    else if (expression.includes("-")) {
      let parts = expression.split("-");
      document.getElementById("display").value = Number(parts[0]) - Number(parts[1]);
    } 
    else if (expression.includes("*")) {
      let parts = expression.split("*");
      document.getElementById("display").value = Number(parts[0]) * Number(parts[1]);
    } 
    else if (expression.includes("/")) {
      let parts = expression.split("/");
      document.getElementById("display").value = Number(parts[0]) / Number(parts[1]);
    } 
    else {
      alert("Invalid Input!");
    }
  }

  function clearDisplay() {
    document.getElementById("display").value = "";
  }
</script>

</body>
</html>
