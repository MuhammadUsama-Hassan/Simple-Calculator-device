# Simple-Calculator-device
JavaaSricpt Assignment # 03
<!DOCTYPE html>
<html>
<head>
    <title>Simple Calculator</title>
    <style>
        body {
            font-family: Arial, sans-serif;
        }
        #calculator {
            
        /* display: flex;
        justify-content: center; */
            width: 600px;
            margin: 0 auto;
            padding: 20px;
            background-color: #52b1dd;
            border: 1px solid #cccccc94;
            border-radius: 5px;
        }
    </style>
</head>
<body>
    <div id="calculator">
        <h2>This calculator will perform simple operations like : + - * /</h2>
        <input type="text" id="num1" placeholder="Enter first number">
        <input type="text" id="num2" placeholder="Enter second number">
        <button onclick="add()">Add</button>
        <button onclick="subtract()">Subtract</button>
        <button onclick="multiply()">Multiply</button>
        <button onclick="divide()">Divide</button>
        <div>
        <h1 id="result">The Answer is: </h1>
    </div>
    </div>

    <script>
        function add() {
            let num1 = parseFloat(document.getElementById("num1").value);
            let num2 = parseFloat(document.getElementById("num2").value);
            document.getElementById("result").innerHTML = "Result: " + (num1 + num2);
        }

        function subtract() {
            let num1 = parseFloat(document.getElementById("num1").value);
            let num2 = parseFloat(document.getElementById("num2").value);
            document.getElementById("result").innerHTML = "Result: " + (num1 - num2);
        }

        function multiply() {
            let num1 = parseFloat(document.getElementById("num1").value);
            let num2 = parseFloat(document.getElementById("num2").value);
            document.getElementById("result").innerHTML = "Result: " + (num1 * num2);
        }

        function divide() {
            let num1 = parseFloat(document.getElementById("num1").value);
            let num2 = parseFloat(document.getElementById("num2").value);
            if (num2 === 0) {
                document.getElementById("result").innerHTML = "Result:Aby saly zero sy kn divid krta hai bay";
            } else {
                document.getElementById("result").innerHTML = "Result: " + (num1 / num2);
            }
        }
    </script>
</body>
</html>
