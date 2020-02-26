# Multiplication_inverse_matrix
행렬의 곱셈은 여러가지 관점에서 바라볼 수 있다.<br>
## 1.row * column
<img src="https://user-images.githubusercontent.com/53939100/75216756-665aca80-57d8-11ea-9bdd-6b8c60e361b9.png"></img><br><br>
행렬의 곱셈은 A 의 row 와 X 의 column 의 곱으로 정의 할 수 있다.<br>
그렇기 떄문에 b 행렬의 3x1 행렬은 A 의 row 3 과 x 의 column 1의 곱으로 표현할 수 있고 다음과 같은 시그마 식이 될 수 있다.<br><br>
<img src="https://user-images.githubusercontent.com/53939100/75217189-9fe00580-57d9-11ea-8e2a-9e62de51b684.png"></img><br><br>
위의 사실들에서 도출해낼수 있는 행렬곱셈의 특징에는 두가지가 있다
#### 1. A 에서의 n 의 크기와 x 에서의 n 의 크기가 일치해야 행렬의 곱셈이 성립할 수 있다.
#### 2. b 행렬의 크기는 m x p 이다.

## 2.column - wise
<img src="https://user-images.githubusercontent.com/53939100/75218021-3d3c3900-57dc-11ea-936b-5fc532542a21.png"></img><br><br>
#### 위 행렬에서 c 행렬은 a행렬 column 의 합으로 나타낼 수 있다.<br>
c11 , c21 , c31 은 각각 a11 과 b11 ,a21 과 b21, a31과 b31 을 원소로 가지고 있다.<br>
그렇기 때문에 c 행렬은 a 의 1,2,3 column 을 b11,b21,b31번 곱한것과 같은 결과를 가지게 된다.<br>
이로인해 Ax=b 에서 b는 A 행렬의 combination 으로 이루어 져 있다는 것을 알 수 있다.

## 3.row - wise
<img src="https://user-images.githubusercontent.com/53939100/75218870-a624b080-57de-11ea-8cf1-2bd1a1ba7c74.png"></img><br><br>
#### 위 행렬에서 c 행렬은 a행렬 row 의 합으로 나타낼 수 있다.<br>
위의 c행렬에서 row 1 은 a 의 row1과 b의 column 들의 조합으로 나타낼 수 있다.<br>
*c11 = a row1 X b column1<br>
*c12 = a row1 X b column2<br>

## column X row
<img src="https://user-images.githubusercontent.com/53939100/75221055-30bbde80-57e4-11ea-8c5d-af3d7f08f496.png"></img><br><br>
위의 column wise 연산과 row wise 연산을 이용하면 위 행렬의 곱셈을 두가지의 행렬의 곱셈으로 나타낼 수 있다.<br>
그런데 그 나눠진 행렬의 곱셈은 두가지 특징을 가진다<br>
<img src='https://user-images.githubusercontent.com/53939100/75221474-454ca680-57e5-11ea-83da-4c1cd4fd5a77.png'></img><br><br>
#### 1.C의 모든 column 은 A column 의 line 에 존재 한다.
#### 2.C의 모든 row 는 x row 의 line 에 존재 한다.
이는 분할된 행렬의 곱셈을 column wise 와 row wise 로 바라보면 검증될 수 있다.<br>
b의 모든 column 은 A column 을 x만큼 곱한것이기 때문에 같은 line 에 존재 할수밖에 없다.<br>
b의 모든 row 는 x row 를 A 만큼 곱한것이기 때문에 같은 line 에 존재 할수밖에없다<br>

# invers matrix
<img src="https://user-images.githubusercontent.com/53939100/75316591-20ba0280-58a9-11ea-9e0e-aa1dd56549f9.png"></img><br><br>
역행렬이란 행렬 A 가 존재할때 곱했을때 단위행렬 I 가 나오는 행렬이다. 역행렬은 위와같이 곱하는 순서가 바뀌어도 성립한다.<br>

## singular case(no inverse)
행렬은 역행렬을 가질수도 있지만 가지지 못하는 경우도 있다. 그러한 경우를 singular case 혹은 no inverse matrix 라고 부른다.<br>
<img src="https://user-images.githubusercontent.com/53939100/75316862-d422f700-58a9-11ea-9b17-6b2dc3d07ae7.png"></img><br><br>
행렬식을 이용하면 위 식은 0이 된다 그렇기 떄문에 역행렬은 존재하지 않는다.<br>
또한 정방행렬 A 가 존재할때, Ax = 0 인 x 를 찾을 수 있다면 A 행렬은 역행렬이 존재하지 않는다.<br>

## Gauss - jordan idea
<img src="https://user-images.githubusercontent.com/53939100/75318658-409ff500-58ae-11ea-93fa-927524be2cfd.png"></img><br><br>
첫번째로, 역행렬을 구하고자 하는 행렬에 단위행렬을 후방 대입시킨다. 그리고 Gauss elimination 을 해준다.<br>
두번째로, pivot 값의 위에있는값을 소거한다.(만약 pivot 값이 1이아니라면 1으로 나눠준다)<br><br>
<img src="https://user-images.githubusercontent.com/53939100/75319140-6974ba00-58af-11ea-96a1-602cef2701de.png"></img><br><br> 위 식을 처음 행렬과 곱해보면 I 행렬이 나오는것을 확인할 수 있다.<br>







