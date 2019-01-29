<h1><a id="Customized_AutoBot_Logo_0"></a>Customized AutoBot Logo</h1>
<p>I updated a new logo of the “Autobots” from the “Transormers” series using HTML and JavaScript.</p>
<p>You can see the live preview clicking on the picture below:<br>
  
<a href="https://negrut112.github.io/JS-creative-AutoBot" target="_blank"><img src="https://i.imgur.com/OUIfXde.png"></a>

<b>HTML</b>
<p>I have used the HTML to define the area where I’m working defining the height, width and the border style:</p>
<p>&lt;canvas id=“myCanvas” height=“310” width=“500” style=“border: 1px solid black”&gt;&lt;/canvas&gt;</p>

<b>JavaScript</b>

<p>Here I applied some graphic methods so I can obtain the desired shapes.</p>
<p>A simple example that helped to generate the “upper eye left area” is:<br>

context.fillStyle=‘black’; // Used to fill the generated path with specific color<br>
context.strokeStyle=‘black’; // Used to generate path before I fill it with specific color</p>
<pre><code>context.beginPath();  // method to start the path<br>
context.moveTo(80,30); // starting point<br>
context.lineTo(130,30); // next defined point<br>
context.lineTo(140,60); // ----//-----<br>
context.lineTo(200,100);<br>
context.lineTo(215,150);<br>
context.lineTo(165,150);<br>
context.lineTo(95,100);<br>
context.lineTo(80,30); // ----//-----<br>
context.fill(); // close the fill method<br>
context.stroke(); // close the stroke method</code></pre>
<p>Conception of the Star was a bit tricky, beacuse is a perfect 5 corner shape, so I had to write the following function using 3 parameters two for starting point and one parameter for side length:</p>
<br>
<pre><code>function filledStar(x,y,a){<br>
context.fillStyle=‘red’<br>
context.beginPath();<br>
context.moveTo(x+a/2-(Math.sin(72<em>Math.PI/180)<em>a/2), y-Math.sin(18</em>Math.PI/180)<em>a/2);/<em>1-ok</em>/<br>
context.lineTo(x+a-2</em>(a/2-(Math.sin(72</em>Math.PI/180)<em>a/2)),y-Math.sin(18</em>Math.PI/180)<em>a/2);/<em>2-ok</em>/<br>
context.lineTo(x+a/2-(Math.sin(36</em>Math.PI/180)<em>a/2),(Math.sin(54</em>Math.PI/180)<em>a/2)+y);/<em>3-ok</em>/<br>
context.lineTo(x+a/2,y-a/2);/<em>4-ok</em>/<br>
context.lineTo(x+a-(Math.sin(36</em>Math.PI/180)<em>a/2),(Math.sin(54</em>Math.PI/180)<em>a/2)+y);/<em>5-ok</em>/<br>
context.lineTo(x+a/2-(Math.sin(72</em>Math.PI/180)<em>a/2),y-Math.sin(18</em>Math.PI/180)*a/2);/<em>6-ok</em>/<br>
context.fill();<br>
context.stroke();<br>
}<br>
console.log();<br>
filledStar(225,50,70);</code></pre>
<p>To perfectly mirror the right side, I used basic calculations, having a middle coordinate point like reference on X-axis.</p>
<p>I’m gonna talk about the colored squares behind the logo, in <a  href="https://negrut112.github.io/JS-Multiple-color-squares/">this</a> project.
