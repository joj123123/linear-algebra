# Linear equation
2x - y = 0<br>
-x + 2y = 3

두개의 식을 행렬로 표현할 수 있음.
이를 위해 3개 요소가 필요

<li>coefficient matrix(A)</li>
<li>unknown vector(X)</li>
<li>right-hand side vector(b)</li><br>

<img src="https://user-images.githubusercontent.com/53939100/74929395-bc1d2480-541e-11ea-9d75-cc3b9bdc1d8f.png"></img><br>
<pre>A     X    b</pre>
으로 표현 가능<br>

# Row picture
row picture 란 행렬을 row 방향으로 방정식을 따져보는것을 의미함<br>
2x - y = 0<br>
-x + 2y = 3<br>
에서는 각각의 방정식이 각각의 row 를 의미함<br>
따라서 해당 방정식의 해는 x=1,y=2이며 이는 두개 방정식의 intersection을 의미함.<br>

# Column picture
column picture 란 해당 행렬에서 x 부분과 y 부분을 따로 보는것이다.<br>
<img src="https://user-images.githubusercontent.com/53939100/74930889-df959e80-5421-11ea-87b1-e306079c693e.png"></img><br>
Column picture 에서는 각각의 행렬을 벡터로 볼 수 있고 각각의 벡터에 b 가 되기위한 x,y 값이 존재할 것이다. <br>

# Linear combination
Linear combination 즉 , 선형 결합은 Column picture 에서의 각 Column(vector) 과 b 에 대한 x,y를 결합시키는 것을 의미한다<br>
즉, Ax = b 가 되는 x 를 찾는 것이고, 이 x 값은 행렬식에 따라 없거나 무한할 수 있다.<br>

# markup
Row picture 로써 행렬 바라본다는것은 방정식으로 바라본다는것<br>
Column picture 로써 행렬을 바라보는것은 행렬을 벡터들의 linear combination 으로 본다는것



