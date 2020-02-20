# singular case
singular case 란 되돌릴 수 없는 행렬을 말한다.<br>
예를들어 Ax = b 의 식에서 b 가 0이되는 경우 b 를 다시 A 로 돌릴 수 없다 따라서 해당 식은 singular case 이다<br>
또한 singular case 는 해가 없거나 무한대로 많 특징을 가지고 있다.<br>
다음은 3 dimension 의 singular case 를 나타낸다<br>
<img src="https://user-images.githubusercontent.com/53939100/74938234-f42d6300-5430-11ea-9add-0448830ba4ef.png"></img><br>

# Elimination
x+2y+z=2<br>
3x+8y+z=12<br>
4y+z=2<br>
다음과 같은 세개의 방정식을 풀때 우리는 변수를 하나씩 제거해가는 방법을 쓸 수 있다.<br>
그렇다면 행렬에서는 어떻게 변수를 제거해나갈까<br>
<br>
<img src="https://user-images.githubusercontent.com/53939100/74939521-5dae7100-5433-11ea-8ca4-46a3e9df8ab2.png"></img><br><br>
다음 행렬에서 1x1 행렬이 0이 아니라면 1x1 을 pivot 값으로 지정한다 <br>
이후 2x1 의 값이 0 이 아니라면 2x1 - a*1x1 = 0 이되는 a 값만큼 row2 에서 row1 을 빼준다 ( row 2 - a * row 1 )<br><br>
<img src="https://user-images.githubusercontent.com/53939100/74939567-7880e580-5433-11ea-950b-779fa31fc461.png"></img><br><br>
또한 2x2 의 값이 0 이 아니라면 2x2 을 두번째 pivot 값으로 지정한다.<br>
그리고 3번째 row 에 대해서도 3x1 을 첫번째 pivot 값을 이용해 없앤 후(해당 예에서는 이미 0이므로 그대로 둔다) 3x2 역시 두번째 pivot 값을 이용해 없앤다.<br>
또한 3x3 의 값이 0 이 아니라면 3x3 을 세번째 pivot 값으로 지정한다.<br><br>
<img src="https://user-images.githubusercontent.com/53939100/74939627-92222d00-5433-11ea-8411-c3ffe4bd5c50.png"></img><br><br>위 이미지는 소거가 모두 완료된 행렬이다, 이와같은 행렬을 U(Upper triangular Matrix) 라고 부른다.<br>

# Failure case
위에서 우리는 행렬의 소거를 진행했다. 하지만 다음과 같이 pivot 값이 0 인 경우 소거법 적용이 불가능 하다. 
<img src='https://user-images.githubusercontent.com/53939100/74941364-3b6a2280-5436-11ea-961d-d63631919160.png'></img><br><br>
또한 첫번째 column 을 소거 했는데 두번째 column 까지 소거되는 경우또한 있을것이다.<br>
이러한 경우 해당 Row 를 아래의 Row 와 바꾸는 방법을 쓸 수 있다.<br>
하지만 다음 Row 의 pivot column 값이 0이라면 바꿔봤자 똑같은 문제에 부딪힐 것이다. 그렇기 때문에<br>
Failure case 는 두가지 case 가 있다<br>
<li> 1. temporary failure (Row exchange 를 통해 극복 가능)</li>
<li> 2. complete failure (pivot = 0 인 상황에서 Row exchange 를 할 수 없는 상황 )</li>








