<!DOCTYPE html>
<html>
<body>
<p id="Problem1"></p>
<p id="Problem2_1"></p>
<p id="Problem2_2"></p>
  
<ip id="Problem3_1"></ip>
<ip id="Problem3_2"></ip>

<script>
var Lucas_Mass= 95;
var Lucas_Height=1.88;
  
var Johan_Mass=85;
var Johan_Height=1.77;
  
var BMI_Lucas= Lucas_Mass /Lucas_Height*Lucas_Height;
  
var BMI_Johan= Johan_Mass /Johan_Height*Johan_Height;
  
var lucasHigerBMI = Boolean(BMI_Lucas >BMI_Johan);
  
document.getElementById("Problem1").innerHTML =lucasHigerBMI;


//Problem 2
  
var C = parseInt(prompt('Enter the temperature in Celsius '));
  
var C_to_F= C*9/5+32;
  
var F = parseInt(prompt('Enter the temperature in fahrenheit '));
  
var F_to_C = (F-32)*5/9;
  
//console.log(`$C C $(C_to_F) F`);
document.getElementById("Problem2_1").innerHTML =C_to_F;
  
//console.log(`$F F $(F_to_C) C`);
document.getElementById("Problem2_2").innerHTML =F_to_C;
  
//Problem 3
  
var Net_1 = parseInt(prompt('Enter the Nets 1 Score '));
var Net_2 = parseInt(prompt('Enter the Nets 2 Score '));
var Net_3 = parseInt(prompt('Enter the Nets 3 Score '));
  
var Knicks_1 = parseInt(prompt('Enter the Knicks 1 Score '));
var Knicks_2 = parseInt(prompt('Enter the Knicks 2 Score '));
var Knicks_3 = parseInt(prompt('Enter the Knicks 3 Score '));
  
var Net_Team_Avg= (Net_1+Net_2+Net_3)/3;
  
var Knicks_Team_Avg= (Knicks_1+Knicks_2+Knicks_3)/3;
  
if(Net_Team_Avg >Knicks_Team_Avg) {
document.getElementById("Problem3_1").innerHTML ="Nets Team Win";
  
}else if (Net_Team_Avg <Knicks_Team_Avg){
document.getElementById("Problem3_1").innerHTML ="Knicks Team Win";
}
else{
document.getElementById("Problem3_1").innerHTML ="Match Draw";
}
  
//for bonus part
  
var Net_Team_Total= Net_1+Net_2+Net_3;
var Knicks_Team_Total=Knicks_1+Knicks_2+Knicks_3;
  
if(Net_Team_Total >=100 && Knicks_Team_Total>=100 ){
//document.write ("<br>");
document.write("\n");
  
if (Net_Team_Total>Knicks_Team_Total){
document.getElementById("Problem3_2").innerHTML ="Nets Team Win";
  
}else if (Net_Team_Total<Knicks_Team_Total) {
document.getElementById("Problem3_2").innerHTML ="Knicks Team Win";
}
  
else{
  
document.getElementById("Problem3_2").innerHTML ="Match Draw"
  
}
  
}
  
  

</script>
</body>
</html>

