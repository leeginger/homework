# 그리드로 애플 사이트 반응형 만들기

[링크] https://leeginger.github.io/homework/apple/apple.html

## 이미지 배율에 대해

> Apple 제품 이미지는 <img> 요소가 아닌 CSS의 background 속성을 활용하여 구현한다.
> 이 때 디바이스의 픽셀 밀도에 따라 1배율 또는 2배율 이미지가 배경으로 반영되도록 한다

이 부분은 어떻게 해야 하는지 모르겠어서 데스크탑 버전에서는 wide 이미지를 쓰고 1024 이하 화면에서는 작은 이미지를 사용했다.

## 반응형

미디어 쿼리를 쓰려다 목요일에 container 쿼리를 배운거같아서 적용해봤다.
내가 반응형을 구현하고싶은 부분의 부모요소에게 container: container / inline-size 라고 적용해줘야한다.

```.main-container {
  display: grid;
  grid-template-columns: repeat(10, 1fr);
  container: container / inline-size;
  gap: 1rem;
```

## 회고

> 나에게 이번 그리드 과제는 너무나 어려웠다.. md에 과정을 써야 하는데 뭘 써야 할지 모르겠다..
> 왜냐면 내가 개념을 제대로 이해하고 만든게 아니기 때문이다.. 그동안 학습하면서 선생님과 함께 만든 코드를 보면서 복붙을 한 것 같고 과제를 시작하기 앞서 참조문서와 회고 팀원들이 보내준 블로그를 많이 읽어보고 퍼블을 시작했다.

> css를 어떻게 하면 깔끔하게 쓸 수 있을까 하다 중첩을 써봤는데 그래도 길어지고 그랬다.

## 참조 문서

https://yamoo9.gitbook.io/css-grid

https://inpa.tistory.com/entry/CSS-%F0%9F%93%9A-%EA%B7%B8%EB%A6%AC%EB%93%9CGrid-%F0%9F%92%AF-%EC%B4%9D%EC%A0%95%EB%A6%AC
