# Celsius-to-Fahrenheit-and-viva
<!DOCTYPE html>
<html>
<head>
<meta name="viewport" content="width=device-width, initial-scale=1">
<style>
body
{
  border:2px solid black;
  padding :10px;
}
.label
{
font-family:bold;
font-size:20px ;
}
.titles
{
  color :white;
  background-color:gray;
}
.inputs
{ 

text-align:left;
font-size :23px ;
border :2px solid black ;
margin-top:10px ;
margin-bottom:10px;
border-radius :5px ;
}
.button {
  padding: 10px 10px;
  font-size: 15px;
  text-align:center;
  cursor: pointer;
  outline: none;
  color:black;
  background-color:skyblue;
  border:10px;
  border-radius:15px;
  box-shadow:5px 5px  5px gray;
}

.button:hover {
background-color:lightgray;
box-shadow:5px 5px  5px gray;
}

.button:active {
  background-color:violet;
  box-shadow:5px 5px gray;
  transform :translate(4px);
}
</style>
</head>
<body>
<h1 class="titles">Fahrenheit to Celsius</h1>
<div>
<label class="label">Fahrenheit number :</label >
  <input type="text" id="input" class="inputs" placeholder="Enter the number">
</div>
<button class="button" onclick="convert1()">Click Me</button>
<div>
  <h1 id="result"></h1>
</div>
<script>
function convert1() 
{ 
  const input = Number(document.getElementById("input").value);
  const convertval =(input - 32) * 5 / 9;
  const res = document.getElementById("result");
  res.innerHTML = convertval.toFixed(2);  
}
</script>
<hr>
<!--celsius to Fahrenheit -->
<h1 class="titles">Celsius to Fahrenheit</h1> <!-- Corrected the heading -->
<div>
<label class="label">Celsius number :</label >
  <input type="text" id="input2" class="inputs" placeholder="Enter the number">
</div>
<button class="button" onclick="convert2()">Click Me</button>
<div>
  <h1 id="result2"></h1>
</div>
<script>
function convert2() 
{ 
  const input2= Number(document.getElementById("input2").value);
  const convertval =(input2* 1.8)+32;
  const res2= document.getElementById("result2");
  res2.innerHTML = convertval.toFixed(2);  
}
</script>
</body>
</html>
