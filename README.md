# Ex.08 Design of a Standard Calculator
## Date: 09/11/2023

## AIM:
To design a web application for a standard calculator with minimum five operations.

## DESIGN STEPS:

### Step 1:
Clone the github repository and create Django admin interface.

### Step 2:
Change settings.py file to allow request from all hosts.

### Step 3:
Use CSS for creating attractive colors.

### Step 4:
Write JavaScript program for implementing five different operations.

### Step 5:
Validate the HTML and CSS code.

### Step 6:
Publish the website in the given URL.

## PROGRAM :
```
<!DOCTYPE html>
<html>
<head>
  <title>Calculator</title>
  <style>
    input[type="text"] {
      width: 400px;
    }
  </style>
</head>
<body>
  <h1>Calculator</h1>
  <input type="text" id="display" disabled>
  <br>
  <button onclick="appendToDisplay('1')">1</button>
  <button onclick="appendToDisplay('2')">2</button>
  <button onclick="appendToDisplay('3')">3</button>
  <button onclick="appendToDisplay('+')">+</button>
  <br>
  <button onclick="appendToDisplay('4')">4</button>
  <button onclick="appendToDisplay('5')">5</button>
  <button onclick="appendToDisplay('6')">6</button>
  <button onclick="appendToDisplay('-')">-</button>
  <br>
  <button onclick="appendToDisplay('7')">7</button>
  <button onclick="appendToDisplay('8')">8</button>
  <button onclick="appendToDisplay('9')">9</button>
  <button onclick="appendToDisplay('*')">*</button>
  <br>
  <button onclick="appendToDisplay('0')">0</button>
  <button onclick="clearDisplay()">C</button>
  <button onclick="calculateResult()">=</button>
  <button onclick="appendToDisplay('/')">/</button>

  <script>
    function appendToDisplay(value) {
      document.getElementById('display').value += value;
    }

    function clearDisplay() {
      document.getElementById('display').value = '';
    }

    function calculateResult() {
      try {
        document.getElementById('display').value = eval(document.getElementById('display').value);
      } catch (error) {
        document.getElementById('display').value = 'Error';
      }
    }
  </script>
</body>
</html>
```

## OUTPUT:
![cal](https://github.com/jaswanth-1723/Calc/assets/127680667/90bd974a-ae58-4a91-976d-43fd436375cf)

## RESULT:
The program for designing a standard calculator using HTML and CSS is executed successfully.
