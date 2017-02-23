# Canvas HTML5 + JS

## - Setup
Get Canvas by ID:
var doc = document.getElementById("#canvas");

### Canvas it self has properties some of does properties you can get by
doc.canvas.ID || doc.canvas.width || doc.canvas.height

### Too create objects like a rectangular
#####     X position , Y position , W Width, h Height
doc.fillRect (x,y,w,h) <br>
doc.fillRect (x,y,w,h) #### Two .fillRect will create two rectangulares  <br>
doc.strokeRect (x , y , w ,h ) will create a stroke around the rectangular - x ,y needs to be equal to the x , y of the rectangular you want to add a stroke too. <br>
doc.fillStyle = "color || hex || rgba() || gradient || pattern <br>
doc.clearRect (x , y ,w ,h) If Width and Height (x,y) equal to canvas.width and height it will clear all canvas, if its equal to a rectangular X, Y, W ,H will clear that rectangular. <br>
doc.createLinearGradient (x0, y0 , x1 ,y1): again position and sizes; <br>
doc.addColorStop (0, "color"); Gradient starts color = 0 <br>
doc.addColorStop (1, "color");  Gradient end color = 1 <br>
doc.createRadialGradient(x0, y0 ,r0, x1 ,y1, r1); <br>
doc.createPattern("url to pattern? ", "repeat"); <br>
doc.fill(); // to fill pattern <br>

### Lines

doc.beginPath();<br>
doc.lineWidth = 20;<br>
doc.lineCap = "round"; <br>
doc.lineJoin = "miter";<br>
doc.miterLimit = 5;<br>
doc.setLineDash([20,10]); Width of dash and Margin between dash<br>
doc.lineDashOffset = 50; // will move the offset of the element - used to animations ? <br>

doc.moveTo(150,150); // Start Point <br>
doc.lineTo(240,240); // Draw first line to <br>
doc.lineTo(3000,40); // keep drawing to <br>
doc.stroke(); <br>
