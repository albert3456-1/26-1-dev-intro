# margin
margin은 **상하좌우에 여백을 남겨놓는 방법**이다.
(바깥쪽여백)
margin값에 숫자(px)를 나열하면 다음과 같은 방식으로 설정된다.
- 1개 : 상하좌우 여백
- 2개 : 상하 여백, 좌우 여백
- 3개 : 상 여백, 좌우 여백, 하 여백
- 4개 : 상 여백, 우 여백, 좌 여백, 하 여백

```
.inner_area {
  margin: 40px;
}

.inner_area {
  margin: 40px 20px;
}

.inner_area {
  margin: 40px 20px 30px;
}

.inner_area {
  margin: 40px 20px 30px 50px;
}
```
그 외에도 각 속성값을 지정해줄 수도 있다.
```
.inner_area {
  margin-top: 40px;
  margin-right: 20px;
  margin-bottom: 30px;
  margin-left: 50px;
}
```
# padding
padding은 **글자의 배경을 맞춰 채워넣는 방법**이다.(안쪽여백)
사용방법과 순서는 마진이랑 유사하다.
```
p {
padding: 5px 7px 3px 0px;
}
```
각 요소 설정도 동일하다.
```
p {
padding-top: 5px;
padding-right: 5px;
padding-bottom: 5px;
padding-left: 5px;
}
```

참고로 px뿐만 아니라 cm, % 도 가능하며, margin은 음수값이 가능하지만, padding은 불가하다

[margin](https://frontendstory.tistory.com/9).
[padding](https://aboooks.tistory.com/81).