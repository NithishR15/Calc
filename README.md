# Ex.08 Design of a Standard Calculator
## Date:14/12/2023

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
<html>
<head>
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <center>
        <h1>SIMPLE CALCULATOR</h1>
        <h1>NITHISH R (23006406)</h1>
    </center>
    <style type="text/css">
        *{
            margin: 0;
            padding: 0;
            font-family: Arial, Helvetica, sans-serif;
            box-sizing: border-box;
        }
        .container {
            width: 100%;
            height: 100vh;
            background: rgb(84, 89, 225);
            display: flex;
            align-items: center;
            justify-content: center;
        }
        .calculator {
            background: rgb(11, 226, 154);
            padding: 20px;
            border-radius: 10px;
        }
        .calculator form input {
            border: 0;
            outline: 0;
            width: 60px;
            height: 60px;
            border-radius: 10px;
            box-shadow: -8px -8px 15px rgba(180, 180, 180, 0.1),  5px 5px 15px rgba(0, 0, 0, 0.2);
            background: black;
            font-size: 20px;
            color: white;
            cursor: pointer;
            margin: 10px;
        }
        form .enter {
            display: flex;
            justify-content: flex-end;
            margin: 20px 0;
        }
        form .enter input {
            text-align: right;
            flex: 1;
            font-size: 45px;
            box-shadow: none;
            border: 1px solid rgb(2, 245, 245);
            padding: 20px;
        }
        form input.equal {
            width: 145px;
        }
        form input.color {
            color: rgb(255, 0, 0);
        }
    </style>
</head>
<body>
    <div class="container">  
        <div class="calculator">
            <form>
                <div class="enter">
                    <input type="text" name="display">
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
    </div>
</body>
</html>


```
## OUTPUT:
![Alt text](calculator.png)

## RESULT:
The program for designing a standard calculator using HTML and CSS is executed successfully.
