<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="styles.css">
    <title>Counter  App</title>
</head>
<body>
  #green {
    color: green;
    text-align: center;
}

body {
    text-align: center;
}

.clicks {
    display: flex;
    justify-content: center;
}
    <h1>Counter App</h1>
    <p id="green">This is a counting game. It is aimed at creating a counting session which adds and subtracts values using a button.<br>
    C'mon play it with me.</p>
    <p id="numeral">0</p>
    <div class="clicks">
    <button id="first">Increase</button>
    <button id="reset">Reset</button>
    <button id="second">Decrease</button>
    </div>
    <script src="script.js">   
      
let output = 0;
const numeral = document.getElementById("numeral");
numeral.textContent = output;

const addButton = document.getElementById("first");
const resetButton = document.getElementById("reset");
const subtractButton = document.getElementById("second");

addButton.addEventListener("click", function(){
  output += 1;
  numeral.textContent = output;
});

subtractButton.addEventListener("click", function() {
  output -= 1;
  numeral.textContent = output;
});

resetButton.addEventListener("click", function() {
  alert("This game has been resetted");
  output = 0;
  numeral.textContent = output;
});
    </script>
</body>
</html>


