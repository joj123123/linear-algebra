# Matrix_Notation_Multiplication
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
그렇기 때문에 c 행렬은 a 의 1,2,3 column 을 b11,b21,b31번 곱한것과 같은 결과를 가지게 된다.

## row - wise
<img src="https://user-images.githubusercontent.com/53939100/75218870-a624b080-57de-11ea-8cf1-2bd1a1ba7c74.png"></img><br><br>
위의 c행렬에서 row 1 은 a 의 row1과 b의 column 들의 조합으로 나타낼 수 있다.<br>
*c11 = a row1 X b column1<br>
*c12 = a row1 X b column2<br>





