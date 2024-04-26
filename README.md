# Ex.08 Design of a Standard Calculator
## Date: 26/04/2024

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

cal.html
```
<html lang="en">
<head>
    <title>CALCULATOR</title>
<script>
function fn(e){
    if (e.innerHTML == '=') {
        output. value = eval (output.value);
}
else if (e.id == 'back') {
    v = output. value;
    output. value = v.substring(0, v.length - 1);
}
else if (e. innerHTML == 'C') {
    output. value = '';
}
else {
    output.value += e.innerHTML;
}
}
</script>
<link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-QWTKZyjpPEjISv5WaRU9OFeRpok6YctnYmDr5pNlyT2bRjXh0JMhjY6hW+ALEwIH" crossorigin="anonymous">
<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap-icons@1.11.3/font/bootstrap-icons.min.css">
</head>
<body>
    <div class="bg-warning mx-auto text-center text-green" style="width: 24rem;"><b>SAI SANJAY R</b></div>
    <div class="bg-warning mx-auto text-center text-pink" style="width: 24rem;"><b>212223040178</b></div>
    <div class="bg-warning row mx-auto text-center" style="width: 24rem;" >
         <div class="col-12 my-4"><input type="text" name="" id="output" style="width: 100%;height: 50px;border-radius: 25px;"></div> 
            <div class="m-3 col-2 btn btn-primary rounded-4" onclick="fn(this)" >(</div> 
            <div class="m-3 col-2 btn btn-primary rounded-4" onclick="fn(this)">)</div> 
            <div class="m-3 col-2 btn btn-danger rounded-4" onclick="fn(this)">C</div> 
            <div class="m-3 col-2 btn btn-danger rounded-4" onclick="fn(this)" id="pink"><i class="bi bi-backspace"></i>
</div>
<div class="m-3 col-2 btn btn-success rounded-4" onclick="fn(this)">7</div>
<div class="m-3 col-2 btn btn-success rounded-4" onclick="fn(this)">8</div>
<div class="m-3 col-2 btn btn-success rounded-4" onclick="fn(this)">9</div> 
<div class="m-3 col-2 btn btn-primary rounded-4" onclick="fn(this)">*</div>
<div class="m-3 col-2 btn btn-success rounded-4" onclick="fn(this)">4</div>
<div class="m-3 col-2 btn btn-success rounded-4" onclick="fn(this)">5</div>
<div class="m-3 col-2 btn btn-success rounded-4" onclick="fn(this)">6</div>
<div class="m-3 col-2 btn btn-primary rounded-4" onclick="fn(this)">-</div>
<div class="m-3 col-2 btn btn-success rounded-4" onclick="fn(this)">1</div> 
<div class="m-3 col-2 btn btn-success rounded-4" onclick="fn(this)">2</div>
<div class="m-3 col-2 btn btn-success rounded-4" onclick="fn(this)">3</div>
<div class="m-3 col-2 btn btn-primary rounded-4" onclick="fn(this)">+</div>
<div class="m-3 col-2 btn btn-success rounded-4" onclick="fn(this)">0</div>
<div class="m-3 col-2 btn btn-success rounded-4" btn-success onclick="fn(this)">.</div>
<div class="m-3 col-2 btn btn-primary rounded-4" onclick="fn(this)">%</div>
<div class="m-3 col-2 btn btn-primary rounded-4" onclick="fn(this)">/</div> 
<div class="m-3 col-11 btn btn-dark rounded-4" onclick="fn(this)">=</div>
</div>
</body>
</html>
```
index.js
```
function display(value){
    document.getElementById("result").value+=value;
 }
  function clear(){
     document.getElementById("result").value='';
  }
  function solve(){
    let x = document.getElementById('result').value
    let y = eval(x);
    document.getElementById('result').value = y
    return y
}
```
style.css
```
table{
    border: 5px solid black;
    margin-left:auto;
    margin-right: auto;
    
}
input[type="text"]{
    border: 3px solid black;
    padding: 20px 30px;
    font-size: 24px;
    font-weight: bold;
    border-radius: 20px;
    background-color: bisque;
}


input[type="button"]{
    width: 100%;
    padding: 20px 40px;
    background-color:rgb(60, 207, 230);
    border-radius: 10px;
    font-size: medium;
}
```


## OUTPUT:
![c:\Users\admin\Pictures\Screenshots\Screenshot 2024-04-26 185415.png](<Screenshot 2024-04-26 185415.png>)
![alt text](<Screenshot 2024-04-26 185427.png>)


## RESULT:
The program for designing a standard calculator using HTML and CSS is executed successfully.
