> # TIL - 2021-03-17

## 💡 *input()* 과 *readline()* 차이!
<hr/>

 > 문제분석

- 알고리즘 문제를 풀다보면 input()사용시 시간초과가 나오던걸 readline() 으로 바꿔주면 해결 되는 것을 간간히 볼 수 있다.
- Python3 에서 input()은 입력 값을 문자열로 받게 된다.
- 그렇다면 input()은 왜 느릴까

> input vs readline
- 일단 readline과 input()은 같은 역활을 하지 않는다.
- input()은 입력받기전 prompt message을 출력해야 하며 그로인해 약간의 부하가 생겨 시간이 걸릴 수 있다.
- 반면 readline은 prompt message를 인수로 받지 않는다.

- 또한 input() 은 입력 받은 값의 개행문자를 삭제시키지만 readline은 개행문자를 삭제 하지 않는다.
- 해서 readline으로 입력받고 바로 그대로 출력을 해보면 뒤에 이상한문자가 같이 찍히는걸 볼수 있다.

> 요약

    'input()'은 입력을 받고 -> 문자열로 변환 -> 추가 strip 진행  
<br/>

- input 과 readline의 가장 큰 차이는 input은 내장 함수로 취급되고 readline은 sys메소드라서 file object로 취급

