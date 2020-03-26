# column space dimension = row space dimension proof
~~~
     [1,1,2]       [1,1]     [1,0,1]  
     [2,3,5]   =   [2,3]     [0,1,1]
     [3,4,7]       [3,4]
     
        A      =     B     X    C
      (m x n)      (m x k)    (k x n)
~~~
A 행렬은 B(basis columns of A) 와 C(coefficient of B) 행렬의 곱으로 나타낼 수 있다.
이를 column space 에서 바라보면 B의 Columns 들의 linear combination 으로 A의 column space를 설명할 수 있다. 이때에, column space of A 는 B 행렬의 column 의 수, 즉 k 개가 된다.
반대로, C 의 row space 를 바라보면, A 의 row space 는 C 의 row space 의 linear combination 으로 이루어 지는것을 볼 수 있다(이때에는 B가 coefficient 가 된다고 생각하면 편함)
C의 row space는 C 의 rows 가 basis 일수도, 아닐수도 있다. 즉, 밑의 식이 성립한다.
row space <= column space
그런데, 이를 A Transpose 로 또다시 해보면,
column space <= row space 가 된다.
즉, row space = column space 인 것이다.

