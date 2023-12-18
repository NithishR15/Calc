# Ex.08 Design of a Standard Calculator
## Date:15/12/2023

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
calculator.html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <title>Simple Calculator</title>
    <style>
        body {
            background-color: #05f9ed;
            font-family: Arial, sans-serif;
            display: flex;
            align-items: center;
            justify-content: center;
            height: 100vh;
            margin: 0;
            flex-direction: column;
            justify-content: space-evenly;
    
        }

        #calculator {
           background-color:red;
            border: 2px solid #f90505;
            border-radius: 10px;
            padding: 20px;
            text-align: center;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
        }

        input[type="text"] {
            width: 100%;
            padding: 10px;
            margin-bottom: 10px;
            font-size: 18px;
        }

        input[type="button"] {
            width: 48px;
            height: 48px;
            font-size: 18px;
            margin: 5px;
            cursor: pointer;
        }

        input[type="button"]:hover {
            background-color: #e80d0d;
        }

        #clear {
            background-color: #3eec55;
            color: #fff;
        }
        .container{
            border: 8px solid #f90505;
            background-color: #3eeca6;
            padding: 20px;
        }
        .enter{
            margin-right: 50px;
        }
        
    </style>
</head>
<body>
<div class="name">
    <h1>SIMPLE CALCULATOR</h1>
    <h1>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;NITHISH R</h1>
</div>
<div class="container">  
    <div class="calculator">
        <form>
            <div class="enter">
                <input type="text" name="display" placeholder="Enter a value">
            </div>
            <div>
                <input type="button" onclick="display.value=''" value="AC" class="color">
                <input type="button" onclick="display.value=display.value.toString().slice(0,-1)" value="Del" class="color">
                <input type="button" onclick="display.value+='%'" value="%" class="color">
                <input type="button" onclick="display.value+='/'" value="/" class="color">
            </div>
            <div>
                <input type="button" onclick="display.value+='7'" value="7">
                <input type="button" onclick="display.value+='8'" value="8">
                <input type="button" onclick="display.value+='9'" value="9">
                <input type="button" onclick="display.value+='*'" value="*" class="color">
            </div>
            <div>
                <input type="button" onclick="display.value+='4'" value="4">
                <input type="button" onclick="display.value+='5'" value="5">
                <input type="button" onclick="display.value+='6'" value="6">
                <input type="button" onclick="display.value+='-'" value="-" class="color">
            </div>
            <div>
                <input type="button" onclick="display.value+='1'" value="1">
                <input type="button" onclick="display.value+='2'" value="2">
                <input type="button" onclick="display.value+='3'" value="3">
                <input type="button" onclick="display.value+='+'" value="+" class="color">
            </div>
            <div>
                <input type="button" onclick="display.value+='0'" value="0">
                <input type="button" onclick="display.value+='.'" value="." class="color">
                <input type="button" onclick="display.value=eval(display.value)" value="=" class="equal color">
            </div>
        </form>
    </div>
    <script>
        function addToDisplay(value) {
            document.getElementById('display').value += value;
        }
    
        function clearDisplay() {
            document.getElementById('display').value = '';
        }
    
        function calculate() {
            try {
                document.getElementById('display').value = eval(document.getElementById('display').value);
            } catch (error) {
                document.getElementById('display').value = 'Error';
            }
        }
    </script>
    
    
</div>
</body>
</html>


```
## OUTPUT:
![Alt text](<Screenshot (40).png>)

## RESULT:
The program for designing a standard calculator using HTML and CSS is executed successfully.
