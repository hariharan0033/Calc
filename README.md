# Ex.08 Design of a Standard Calculator
## Date: 21/04/2024

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
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Calculator</title>
    <style>
        .out-container{
            width: 25%;
            margin: auto;
            margin-top: 3rem;
            background-color: rgb(75, 75, 75);
            text-align: center;
            color: white;
            font-weight: bold;
            font-size: 2rem;
            padding: 15px;
            padding-bottom: 30px;
            border-radius: 30px;
            height: 70%;
        }
        .inp{
            width: 90%;
            height: 2rem;
            margin: 5px;
            border-radius: 15px;
            border: none;
        }
        .btn-container{
            display: flex;
            flex-direction: row;
            justify-content: space-around;
        }
        .btn{
            width: 4rem;
            height: 4rem;
            padding: 5px;   
            margin:10px auto;
            cursor: pointer;
            display: grid;
            place-content:center;
            border-radius: 50%;
        }

        .yellow{
            background-color: rgb(255, 187, 0);
            width: 90%;
            margin: 5px auto;
            border-radius: 15px;
            height: 3rem;
        }
        .blue{
            background-color: rgb(115, 115, 255);
        }
        .red{
            background-color: rgb(253, 66, 66);
        }
        .green{
            background-color: rgb(35, 174, 35);
        }
        h5{
            margin: 15px auto;
        }
        .inp{
            font-size: 2rem;
            padding: 10px 5px; 
        }
    </style>
</head>
<body>
    <div class="out-container">
        <h5>HARIHARAN E (212221040052)</h5>
        <input type="text" name="" id="inp" class="inp">
        
        <div class="btn-container">
            <div onclick = "fn(this)" class="btn blue">(</div>
            <div onclick = "fn(this)" class="btn blue">)</div>
            <div onclick = "fn(this)" class="btn red">C</div>
            <div onclick = "fn(this)" class="btn red" id="back">&lt;</div>
        </div>

        <div class="btn-container">
            <div onclick = "fn(this)" class="btn green">1</div>
            <div onclick = "fn(this)" class="btn green">2</div>
            <div onclick = "fn(this)" class="btn green">3</div>
            <div onclick = "fn(this)" class="btn blue">/</div>
        </div>

        <div class="btn-container">
            <div onclick = "fn(this)" class="btn green">4</div>
            <div onclick = "fn(this)" class="btn green">5</div>
            <div onclick = "fn(this)" class="btn green">6</div>
            <div onclick = "fn(this)" class="btn blue">*</div>
        </div>

        <div class="btn-container">
            <div onclick = "fn(this)" class="btn green">7</div>
            <div onclick = "fn(this)" class="btn green">8</div>
            <div onclick = "fn(this)" class="btn green">9</div>
            <div onclick = "fn(this)" class="btn blue">-</div>
        </div>

        <div class="btn-container">
            <div onclick = "fn(this)" class="btn green">0</div>
            <div onclick = "fn(this)" class="btn green">.</div>
            <div onclick = "fn(this)" class="btn blue">%</div>
            <div onclick = "fn(this)" class="btn blue">+</div>    
        </div>
        <div class="btn yellow" onclick = "fn(this)">=</div>

    </div>

    <script>
        const fn = (e) => {
            if(e.innerHTML =="="){
                inp.value = eval(inp.value);
            }
            else if(e.innerHTML =="C"){
                inp.value = "";
            }
            else if(e.id=="back"){
                data = inp.value;
                inp.value = data.substring(0,data.length-1);
            }
            else{
                inp.value += e.innerHTML;
            }
        }
    </script>
</body>
</html>
```
## OUTPUT:
![Screenshot (230)](https://github.com/hariharan0033/Calc/assets/125666185/c0855abb-f76b-445a-86d9-8d65abfbab03)

![Screenshot (231)](https://github.com/hariharan0033/Calc/assets/125666185/a7216227-1578-4bb4-b9ac-b43759706e03)



## RESULT:
The program for designing a standard calculator using HTML and CSS is executed successfully.
