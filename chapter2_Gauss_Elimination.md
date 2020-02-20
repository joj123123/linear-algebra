# singular case
singular case 란 되돌릴 수 없는 행렬을 말한다.<br>
예를들어 Ax = b 의 식에서 b 가 0이되는 경우 b 를 다시 A 로 돌릴 수 없다 따라서 해당 식은 singular case 이다<br>
또한 singular case 는 해가 없거나 무한대로 많은 특징을 가지고 있다.<br>
다음은 3 dimension 의 singular case 를 나타낸다<br>
<img src="https://user-images.githubusercontent.com/53939100/74938234-f42d6300-5430-11ea-9add-0448830ba4ef.png"></img><br>

# Elimination
x+2y+z=2<br>
3x+8y+z=12<br>
4y+z=2<br>
다음과 같은 세개의 방정식을 풀때 우리는 변수를 하나씩 제거해가는 방법을 쓸 수 있다.<br>
그렇다면 행렬에서는 어떻게 변수를 제거해나갈까<br>

<img src="https://user-images.githubusercontent.com/53939100/74939521-5dae7100-5433-11ea-8ca4-46a3e9df8ab2.png"></img><br>
다음 행렬에서 1x1 행렬이 0이 아니라면 1x1 을 pivot 값으로 지정한다 <br>
이후 2x1 의 값이 0 이 아니라면 2x1 - a*1x1 = 0 이되는 a 값만큼 row2 에서 row1 을 빼준다 ( row 2 - a * row 1 )<br>
<img src="https://user-images.githubusercontent.com/53939100/74939567-7880e580-5433-11ea-950b-779fa31fc461.png"></img><br>
또한 2x2 의 값이 0 이 아니라면 2x2 을 두번째 pivot 값으로 지정한다.<br>
그리고 3번째 row 에 대해서도 3x1 을 첫번째 pivot 값을 이용해 없앤 후 3x2 역시 두번째 pivot 값을 이용해 없앤다.<br>
또한 3x3 의 값이 0 이 아니라면 3x3 을 세번째 pivot 값으로 지정한다.<br>
<img src="https://user-images.githubusercontent.com/53939100/74939627-92222d00-5433-11ea-8411-c3ffe4bd5c50.png"></img><br>


