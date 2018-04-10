# Canvas

#### 路径操作

|函数|备注|
|---|---|
|moveTo(X, Y)|起点|
|lineTo(X, Y)|连接点|
|strokeStyle = 'red'|画线颜色|
|stroke()|画线|
|fillStyle = 'pink'|填充颜色|
|fill()|填充|
|beginPath()|新路径的开始，清除之前路径|
|closePath()|闭合路径|
|strokeRect(X, Y, width, height)|线画矩形|
|fillRect(X, Y, width, height)|填充矩形|
|clearRect(X, Y, width, height)|清除矩形(擦除)|
|requestAnimationFrame(fn)||

````javascript
  let canvas = document.getElementById('canvas');
  let gd = canvas.getContext('2d');

  gd.moveTo(20, 20);
  gd.lineTo(40, 40);
  gd.strokeStyle = 'red';
  gd.stroke();

  gd.beginPath();  //新的路径初始化，清除之前的路径
  gd.moveTo(60, 20);
  gd.lineTo(80,40);
  gd.lineTo(60,40);
  gd.closePath();
  gd.strokeStyle = 'pink';
  gd.stroke();
  gd.fillStyle = 'green';
  gd.fill()
  
  
````
 