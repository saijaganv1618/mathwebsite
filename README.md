# Web Page for Mathematical Calculations

## AIM:

To design a static website with validation to perform mathematical calculations in client side.

## DESIGN STEPS:

### Step 1:

Requirement collection.

### Step 2:

Creating the layout using HTML and CSS.

### Step 3:

Write javascript to perform the calculations.

### Step 4:

Include regularexpression based input validation.

### Step 5:

Validate the layout in various browsers.

### Step 6:

Validate the HTML code.

### Step 6:

Publish the website in the given URL.

## PROGRAM :
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Volume</title>
    <style>
        *{
            box-sizing: border-box;
            font-family: Arial, Helvetica, sans-serif;
        }
        body{
            background-color: orange;
            color:yelloww;
        }
        .container{
            width: 1080px;
            margin-left: auto;
            margin-right: auto;
            background-color: bisque;
            border: yellow;
        }
        .content{
            display: block;
            width: 100%;
            background-color:yellow;
            margin-top: 40px;
            min-height: 400px;
        }
        .text{
            text-align: center;
            padding-top: 50px;
            text-decoration: underline;
        }
        .formelement{
            text-align: center;
            font-family: Georgia, 'Times New Roman', Times, serif;
            font-size: 25px;
            margin-top: 5px;
            margin-bottom: 5px;

        }
        .content2{
            display: block;
            width: 100%;
            background-color:yellow;
            margin-top: px;
            min-height: 400px;
        }
    </style>

</head>


<body>
    <div class="container">
        <div class="content">
            <h1 class="text">Calculating the volume of the cylinder</h1>
            <form>
                <div class="formelement"><label for="aEdit">Height:</label>
                    <input type="text" id="aEdit" value="0"/>
                </div>
                
                <div class="formelement">
                    <label for="bEdit">Radius:</label>
                    <input type="text" id="bEdit" value="0"/>
                </div>
                <div class="formelement">
                    <input type="button" value="Calculate" id="AddButton"/>
                </div>
                
                <div class="formelement">
                    <label for="cEdit">Volume:</label>
                    <input type="text" id="cEdit" value="0" readonly />
                </div>
            </form>

        </div>
        <div class="content2">
            <h1 class="text">Calculating the volume of the Cone</h1>
            <form>
                <div class="formelement"><label for="hEdit">Height:</label>
                    <input type="text" id="hEdit" value="0"/>
                </div>
                
                <div class="formelement">
                    <label for="rEdit">Radius:</label>
                    <input type="text" id="rEdit" value="0"/>
                </div>
                <div class="formelement">
                    <input type="button" value="Calculate" id="AddButton1"/>
                </div>
                
                <div class="formelement">
                    <label for="vEdit">Volume:</label>
                    <input type="text" id="vEdit" value="0" readonly />
                </div>
            </form>

        </div>
    </div>
    <script type="text/javascript">
        var button,button1;
        button = document.querySelector("#AddButton");
        
        button.addEventListener("click",function(){
            var aText,bText,cText;
            var aVal,bVal,cVal;
            aText=document.querySelector("#aEdit");
            bText=document.querySelector("#bEdit");
            cText=document.querySelector("#cEdit");

            aVal = parseInt(aText.value);
            bVal = parseInt(bText.value);
            cVal = (aVal*bVal*bVal)*22/7;
            cText.value = ""+cVal;
        });
        button1 = document.querySelector("#AddButton1");
        button1.addEventListener("click",function(){
            var aText,bText,cText;
            var aVal,bVal,cVal;
            hText=document.querySelector("#hEdit");
            rText=document.querySelector("#rEdit");
            vText=document.querySelector("#vEdit");

            hVal = parseInt(hText.value);
            rVal = parseInt(rText.value);
            vVal = (22/7*rVal*rVal)*hVal;
            vText.value = ""+vVal;
        });


    </script>
</body>
</html>
--include your code--

## OUTPUT:
![output](1.png)
![output](2.png)
-- include your output screenshots ---

## Result:

Thus a website is designed to perform mathematical calculations in the client side.
