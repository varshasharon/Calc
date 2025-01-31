# Ex.08 Design of a Standard Calculator
## Date:
15.11.2023
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
### index.html
```
<!DOCTYPE html>
<html lang="en">

<head>
   <meta charset="UTF-8">
   <meta name="viewport" content="width=device-width, initial-scale=1.0">
   <title>Simple Calculator</title>
   <script>
      function display(val) {
         document.getElementById('result').value += val;
      }
      function Solve() {
         var x = document.getElementById('result').value;
         var y = eval(x);
         document.getElementById('result').value = y;

      }
      function ClearFuntion() {
         document.getElementById('result').value = ''
      }
      function deleteFuntion() {
         var temp = ''
         temp = document.getElementById('result').value;
         var len = temp.length;
         temp = temp.substring(0, len - 1)
         document.getElementById('result').value = temp;
      }

   </script>
   <style>
    .h2{
        font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        font-size: 18px;
    }
      .calc {
        max-width: 500px;
        margin: 500px;
         padding: 20px;
         border: 1px solid bisque;
         border-radius: 10px;
         text-align: center;
         background-color: rgb(244, 234, 191);
      }
      #opButton {
         background-color: rgb(245, 212, 114);
      }

      #deleteButton {
         background-color: rgb(111, 92, 255);
      }

      #clearButton {
         background-color: rgb(184, 177, 245);
      }
      #result {
         border-radius: 5px;
         height: 45px;
         padding-left: 20px;
         color: black;
         font-size: 28px;
         font-weight: 500;
      }
      #numButton,
      #opButton,
      #EqualButton,
      #clearButton,
      #deleteButton {
        margin: 10px;
        font-size: 18px;
        border-radius: 30px;
         padding: 25px;
         border: 1px solid burlywood;
      }


   </style>
</head>

<body>
   <div class="calc">
    <h2>Simple Calculator</h2>
    <input type="text" id="result" />
      <div>
         <input type="button" id="numButton" value="7" onclick="display('7')" />
         <input type="button" id="numButton" value="8" onclick="display('8')" />
         <input type="button" id="numButton" value="9" onclick="display('9')" />
         <input type="button" id="opButton" value="/" onclick="display('/')" />
      </div>
      <div>
         <input type="button" id="numButton" value="4" onclick="display('4')" />
         <input type="button" id="numButton" value="5" onclick="display('5')" />
         <input type="button" id="numButton" value="6" onclick="display('6')" />
         <input type="button" id="opButton" value="*" onclick="display('*')" />
      </div>
      <div>
         <input type="button" id="numButton" value="1" onclick="display('1')" />
         <input type="button" id="numButton" value="2" onclick="display('2')" />
         <input type="button" id="numButton" value="3" onclick="display('3')" />
         <input type="button" id="opButton" value="-" onclick="display('-')" />
      </div>
      <div className='calcu'>
         <input type="button" id="numButton" value="0" onclick="display('0')" />
         <input type="button" id="numButton" value="." onclick="display('.')" />
         <input type="button" id="EqualButton" value="=" onclick="Solve()" />
         <input type="button" id="opButton" value="+" onclick="display('+')" />
      </div>
      <div>
         <input type="button" id='deleteButton' value="Delete" onclick="deleteFuntion()" />
         <input type="button" id="clearButton" onclick="ClearFuntion()" value="Clear" />
      </div>
   </div>
</body>

</html>
```
## OUTPUT:
![output](op1.png)
![output](op2.png)
## RESULT:
The program for designing a standard calculator using HTML and CSS is executed successfully.
