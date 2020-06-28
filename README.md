<!DOCTYPE html>
<html>
<head>
<meta charset="ISO-8859-1">
<title></title>

<style type="text/css">
div{
position: center;
top: 10px;
left: 100px;
width:250px;
height:120px;
border: 2px solid green;
border-radius: 20px;
}
</style>
<script type="text/javascript">
function loginValidation(){
var userName = document.LoginForm.uname.value;
var str=userName.toLowerCase();
var cars = ["rock", "paper", "scissor"];
var m=Math.floor(Math.random() * 3);
var l=cars[m];
while (l==str){
var m=Math.floor(Math.random() * 3);
var l=cars[m];
}
if (str=="rock"){
if (l=="scissor"){
alert("you won");
}
else{
alert("you lost");
}
}
if (str=="paper"){
if (l=="rock"){
alert("you won");
}
else{
alert("you lost");
}
}
if (str=="scissor"){
if (l=="paper"){
alert("you won");
}
else{
alert("you lost");
}
}
}
</script>
</head>
<body>
<form name="LoginForm">
<div>
<br>
<table>
<tr><td>1stuser</td><td> <input type="text" name="uname"/></td></tr>
<tr><td colspan="2" align="Center"><input type="Submit"
value="Result" onClick="loginValidation()"/></td></tr>
</table>
</div>
</form>
</body>
</html>			 
