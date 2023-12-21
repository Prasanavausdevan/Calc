# Ex.08 Design of a Standard Calculator
## Date:20/12/2023

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
~~~
calc.html


<!DOCTYPE html>
<html lang="en">
    <head>
        <center>
            <h1>SIMPLE CALCULATOR</h1>
            <h1>PRASANA V(212223040150)</h1>
           </center>
        <title>Calculator</title>
        
        <script>
        function calculate(args)
        {
            res = document.getElementById("result");
            expression = res.innerText;
            cmd = args.srcElement.innerText;
            if(cmd == "=")
            {
                expression = "" + eval(expression)
            }
            else if(cmd == "C")
            {
                expression=""
            }
            else if(cmd == "DEL")
            {
                expression = expression.slice(0, -1);

            }
            else if(cmd == "√")
            {
                expression = "" + Math.sqrt(eval(expression));
            }
            else if(cmd == "%")
            {
                expression = expression % 1;
            }
            else if(cmd == "log")
             {
        expression = Math.log10(expression);
           }
       
            else{
                expression = expression + cmd;
            }
            res.innerText = expression;
            

        }
         
        </script>
        <center>
        <style>
          
            .calculator-container {
                width: 400px;
                background-color:rgb(59, 53, 181)
                margin: 0 auto; 
                margin-top: 90px;
                text-align: center;
                
            }

           
            button {
                width: 50px;
                height: 50px;
                margin: 10px; 
                font-size: 20px; 
                
                background-color: rgb(120, 15, 15); 
                color: white; 
                border: none;
            }

          
            #result {
                
       background-color:#e5e2ec;
    text-align: right;
    padding-right: 50px;
    font-size: 20px;
    margin-bottom: 20px; 
    border: solid rgb(213, 98, 98) 0.5px;
    color: rgb(73, 56, 165);
    width: 348px;
    height: 50px;
    display: flex;
    align-items: center;
    justify-content: flex-end;

            }
            h1 {
                padding-top: 10px;
                color:white;
                font-size: 50px;
            }
            .redd {
                background-color: rgb(228, 18, 130);
            }
            .bluee {
                
                background-color: rgb(94, 244, 166);
            }
            body {
                background-color: rgb(97, 187, 239);
            }
        </style>

    </head>
<body>
    <div class="calculator-container">
        <h1>CALCULATOR</h1>
        <div id="result">0</div>
        <button onclick="calculate(event);">7</button>
        <button onclick="calculate(event);">8</button>
        <button onclick="calculate(event);">9</button>
        <button class="bluee"  onclick="calculate(event);">/</button>
        <button class="bluee"  onclick="calculate(event);"> DEL </button><br>
        <button onclick="calculate(event);">4</button>
        <button onclick="calculate(event);">5</button>
        <button onclick="calculate(event);">6</button>
        <button class="bluee"  onclick="calculate(event);">*</button>
        <button class="bluee"  onclick="calculate(event);">&radic;</button> </button><br>
        <button onclick="calculate(event);">1</button>
        <button onclick="calculate(event);">2</button>
        <button onclick="calculate(event);">3</button>
        <button class="bluee"  onclick="calculate(event);">-</button>
        <button class="bluee"  onclick="calculate(event);">log</button><br>
        <button onclick="calculate(event);">0</button>
        <button onclick="calculate(event);">.</button>
        <button class="redd" onclick="calculate(event);">C</button>
        <button class="bluee"  onclick="calculate(event);">+</button>
        <button class="bluee" onclick="calculate(event);">=</button><br>
    </div>
    </center>
    </body>
</html>
~~~

## OUTPUT:
![Alt text](<vijay/Screenshot (19).png>)
![Alt text](<vijay/Screenshot (20).png>)



## RESULT:
The program for designing a standard calculator using HTML and CSS is executed successfully.
