<!DOCTYPE html>
<html>
<head>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width">
  <title>Customized AutoBot Logog</title>
</head>
<body>
  <canvas id="myCanvas" height="310" width="500" style="border: 1px solid black"></canvas>
  <script>
  var canvas = document.getElementById('myCanvas');
  var context = canvas.getContext('2d');
  // Blur lines
  for(var i=0;i<25;i++){
    for(var j=0;j<15;j++){
      context.fillStyle='rgb('+ Math.floor(129 - 42*j) + ', 119,'+ Math.floor(50+15*i)+')';
        context.fillRect(i*20+5,j*20+10,8,8);
      }
    }
// Upper Left Eye Area
context.fillStyle='black';
context.strokeStyle='black';
    
context.beginPath();
context.moveTo(80,30);
context.lineTo(130,30);
context.lineTo(140,60);
context.lineTo(200,100);
context.lineTo(215,150);
context.lineTo(165,150);
context.lineTo(95,100);
context.lineTo(80,30);

context.fill();
context.stroke();

//Left Side "Eyes"
context.fillStyle='red';
context.strokeStyle='black';

context.beginPath();
context.moveTo(110,60);
context.lineTo(190,110);
context.lineTo(190,120);
context.lineTo(110,70);
context.lineTo(110,60);

context.fill();
context.stroke();

context.fillStyle='red';
context.strokeStyle='black';

context.beginPath();
context.moveTo(110,60+20);
context.lineTo(190+3,110+20);
context.lineTo(190+3,120+20);
context.lineTo(110,70+20);
context.lineTo(110,60+20);

context.fill();
context.stroke();

//Left Jaw
context.fillStyle='black';
context.strokeStyle='black';

context.beginPath();
context.moveTo(105,135);
context.lineTo(130,153);
context.lineTo(130,173);
context.lineTo(167,188);
context.lineTo(167,270);
context.lineTo(110,230);
context.lineTo(105,135);

context.stroke();
context.fill();

//Mouth
context.fillStyle='black';
context.strokeStyle='black';

context.beginPath();
context.moveTo(215,173);
context.lineTo(183,192);
context.lineTo(183,280);
context.lineTo(193,285);
context.lineTo(215,240);
context.lineTo(300,240);
context.lineTo(322,285);
context.lineTo(332,280);
context.lineTo(332,192);
context.lineTo(300,173);
context.lineTo(300,225);
context.lineTo(215,225);
context.lineTo(215,173);

context.stroke();
context.fill();

//Chin
context.fillStyle='black';
context.strokeStyle='black';

context.beginPath();
context.moveTo(225,255);
context.lineTo(290,255);
context.lineTo(305,285);
context.lineTo(210,285);
context.lineTo(225,255);

context.stroke();
context.fill();

//Nouse
context.fillStyle='black';
context.strokeStyle='black';

context.beginPath();
context.moveTo(240,205);
context.lineTo(275,205);
context.lineTo(275,150);
context.lineTo(290,105);
context.lineTo(257.5,125);
context.lineTo(225,105);
context.lineTo(240,150);
context.lineTo(240,205);

context.stroke();
context.fill();

//Upper Right Eyes Area
context.fillStyle='black';
context.strokeStyle='black';

context.beginPath();
context.moveTo(80+355,30);
context.lineTo(80+355-50,30);
context.lineTo(80+355-60,60);
context.lineTo(80+355-120,100);
context.lineTo(80+355-135,150)
context.lineTo(80+355-130+50,150)
context.lineTo(80+355-130+50+65,100)
context.lineTo(80+355,30)

 context.fill();
context.stroke();

// Right Side "Eyes"
context.fillStyle='red';
context.strokeStyle='black';

context.beginPath();
context.moveTo(405,60);
context.lineTo(405-80,110);
context.lineTo(405-80,120);
context.lineTo(405,70);
context.lineTo(405,60);

context.fill();
context.stroke();

context.fillStyle='red';
context.strokeStyle='black';

context.beginPath();
context.moveTo(405,60+20);
context.lineTo(405+3-80,110+20);
context.lineTo(405+3-80,120+20);
context.lineTo(405,70+20);
context.lineTo(405,60+20);

context.fill();
context.stroke();

//Right Jaw
context.fillStyle='black';
context.strokeStyle='black';

context.beginPath();
context.moveTo(410,135);
context.lineTo(410-25,153);
context.lineTo(410-25,173);
context.lineTo(410-25-37,188);
context.lineTo(410-25-37,270);
context.lineTo(410-25-37+57,230);
context.lineTo(410,135);

context.stroke();
context.fill();

//Forehead
context.fillStyle='black';
context.strokeStyle='black';

context.beginPath();
context.arc(257.5,210,209.2,1.33 * Math.PI,1.67 * Math.PI,false)
context.stroke();
context.fill();

context.beginPath();
context.moveTo(257.5,105);
context.lineTo(160,55);
context.lineTo(150,30);
context.lineTo(365,30);
context.lineTo(355,55);
context.lineTo(257.5,105);

context.stroke();
context.fill();

//Forehead STAR sign
function filledStar(x,y,a){
context.fillStyle='red'
//context.strokeStyle='grey'
context.beginPath();
context.moveTo(x+a/2-(Math.sin(72*Math.PI/180)*a/2), y-Math.sin(18*Math.PI/180)*a/2);/*1-ok*/
context.lineTo(x+a-2*(a/2-(Math.sin(72*Math.PI/180)*a/2)),y-Math.sin(18*Math.PI/180)*a/2);/*2-ok*/
context.lineTo(x+a/2-(Math.sin(36*Math.PI/180)*a/2),(Math.sin(54*Math.PI/180)*a/2)+y);/*3-ok*/
context.lineTo(x+a/2,y-a/2);/*4-ok*/
context.lineTo(x+a-(Math.sin(36*Math.PI/180)*a/2),(Math.sin(54*Math.PI/180)*a/2)+y);/*5-ok*/
context.lineTo(x+a/2-(Math.sin(72*Math.PI/180)*a/2),y-Math.sin(18*Math.PI/180)*a/2);/*6-ok*/
context.fill();
//context.stroke();
}
console.log();
filledStar(225,50,70);
  </script>
</body>
</html>
