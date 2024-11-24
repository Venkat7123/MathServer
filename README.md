# Ex.05 Design a Website for Server Side Processing
## Date: 24/11/2024

## AIM:
 To design a website to calculate the power of a lamp filament in an incandescent bulb in the server side. 


## FORMULA:
P = I<sup>2</sup>R
<br> P --> Power (in watts)
<br> I --> Intensity
<br> R --> Resistance

## DESIGN STEPS:

### Step 1:
Clone the repository from GitHub.

### Step 2:
Create Django Admin project.

### Step 3:
Create a New App under the Django Admin project.

### Step 4:
Create python programs for views and urls to perform server side processing.

### Step 5:
Create a HTML file to implement form based input and output.

### Step 6:
Publish the website in the given URL.

## PROGRAM :
```
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Math Server</title>
    <style>
        div {
            margin-top: 12%;
        }

        form {
            width: 450px;
            height: 50;
            border: 2px solid black;
            padding: 50px;
            line-height: 10px;
            font-size: 32px;
            background: rgb(120, 250, 140);
        }
        body{
            background: beige;
        }
        h1{
            color: #fd7d66;
            font-size: 40px;
            margin-top: 0;
            margin-bottom: 10%;
        }
        input{
            border-radius: 15px;
            margin-left: 10px;
            font-size: 32px;
        }
        .i{
            cursor: pointer;
            box-sizing: border-box;
            background-color: #00b9ff;
            padding-left: 100px;
            padding-right: 100px;
        }
        label{
            color: #f7755e;
            font-size: 40px;
            margin-bottom: 10%;
        }
    </style>
    <script>
        function calc(){
            var x=Number(document.getElementById("l").value);
            var y=Number(document.getElementById("b").value);
            document.getElementById('r').innerText ="Power: "+x*x*y +'W'
        }
    </script>
</head>

<body>
    <div>
        <center>
            <form>
                <h1>Power Calculator</h1>
                <input type="text" name="Current" placeholder="Enter Intensity" id="l"><br><br><br><br>
                <input type="text" name="Resistance" placeholder="Enter Resistance " id="b"><br><br><br>
                <input type="button" value="Calculate" onclick="calc()" class="i"> <br><br><br>
                <label id="r"></label>
            </form>
        </center>
    </div>
</body>

</html>
```

## SERVER SIDE PROCESSING:
```
    <script>
        function calc(){
            var x=Number(document.getElementById("l").value);
            var y=Number(document.getElementById("b").value);
            document.getElementById('r').innerText ="Power: "+x*x*y +'W'
        }
    </script>
```

## HOMEPAGE:
![alt text](<Screenshot 2024-11-23 113437.png>)

## RESULT:
The program for performing server side processing is completed successfully.
