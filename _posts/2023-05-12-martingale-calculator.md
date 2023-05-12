
<html>
<head>
  <title>Martingale Calculator</title>
</head>
<body>

<div style="text-align: center">
  <form>
    <label for="fname">Deposit</label><br>
    <input type="number" id="deposit" name="deposit" min="1" max="999999999" placeholder="100">
  </form>
  <button onclick="calculate()">Calculate</button>
  
  <div id="roundedNumber1" style="color:red;"></div>
  <div id="roundedNumber2" style="color:red;"></div>
  <div id="roundedNumber3" style="color:red;"></div>
  <div id="roundedNumber4" style="color:red;"></div>
  <div id="roundedNumber5" style="color:red;"></div>
  <div id="roundedNumber6" style="color:red;"></div>
</div>
</body>
<script>
function calculate() {
  const deposit = document.getElementById("deposit").value;
  const result1 = deposit * 0.011;
  const result2 = result1 * 2.179;
  const result3 = result2 * 2.179;
  const result4 = result3 * 2.179;
  const result5 = result4 * 2.179;
  const result6 = result5 * 2.179;
  const roundedNumber1 = result1.toFixed(2);
  const roundedNumber2 = result2.toFixed(2);
  const roundedNumber3 = result3.toFixed(2);
  const roundedNumber4 = result4.toFixed(2);
  const roundedNumber5 = result5.toFixed(2);
  const roundedNumber6 = result6.toFixed(2);
  document.getElementById("roundedNumber1").innerHTML = roundedNumber1;
  document.getElementById("roundedNumber2").innerHTML = roundedNumber2;
  document.getElementById("roundedNumber3").innerHTML = roundedNumber3;
  document.getElementById("roundedNumber4").innerHTML = roundedNumber4;
  document.getElementById("roundedNumber5").innerHTML = roundedNumber5;
  document.getElementById("roundedNumber6").innerHTML = roundedNumber6;
}
</script>
</html>