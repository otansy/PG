# PG
<html>
<head>
<meta charset="UTF-8">
<title>
山本HG２
</title>
</head>
<body>
プログラム<br>
<hr>
int[]x=new int[100];<br>
int[]y=new int[100];<br>
int i=0;<br>
<br>
void setup(){<br>
  size(500,500);<br>
}<br>
<br>
void draw(){<br>
  int j,k;<br>
  background(255);<br>
  if(i>0){<br>
    for(j=0;j<=i-2;j=j+2){<br>
      line(x[j],y[j],x[j+1],y[j+1]);<br>
    }<br>
  }<br>
  if(i>=1){<br>
    if(i%2==1){<br>
      line(x[i-1],y[i-1],mouseX,mouseY);<br>
    }<br>
  }<br>
  if(keyPressed==true){<br>
    if(key=='s'){<br>
      println("start");<br>
      x[i]=mouseX;<br>
      y[i]=mouseY;<br>
      i=i+1;<br>
      delay(800);<br>
    }<br>
    else if(key=='f'){<br>
      println("finish");<br>
      x[i]=mouseX;<br>
      y[i]=mouseY;<br>
      i=i+1;<br>
      delay(800);<br>
    }  <br>
    else if(key=='g'){<br>
      for(k=0;k<=i-1;k=k+2){<br>
        println("line(",x[k],",",y[k],",",x[k+1],",",y[k+1],");");<br>
      }<br>
      delay(1000);<br>
    }<br>
  }<br>
}<br>
<hr>
使い方<br>
カーソルをはじめの位置に持っていき、キーボードのSを押す。<br>
※この時、コンソールにstartと書かれているかチェック！！<br>
線が出てきたら終わりの位置にカーソルを持っていき、キーボードのFを押す。<br>
※この時、コンソールにfinishと書かれているかチェック！！<br>
線が全て描けたらキーボードのGを押す<br>
そうするとコンソール上にたくさんのline()関数が表示されるので、コピペ<br>
以上！！！！！^_^
