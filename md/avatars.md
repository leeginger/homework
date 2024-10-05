# float와 flex로 각각 만든 이미지 리스트 정렬

## float 정렬

> 1. float:left로 정렬을 하고 이미지들의 간격 사이는 padding을 주었다.
> 2. img 태그에는 img를 감싸는 div나 span태그를 줘야되나 고민하다 마크업이 길어지는게 복잡해보여서 그냥 img태그에 css수정을 했다.
> 3. li 태그에 왜 높이값이 68px로 잡히는지는 알 수 없었다.
> 4. 상태 정보를 제공하기 위해 span에 text를 넣었다가 텍스트를 안보이게 하려고 테일윈드에 있는 .sr-only css를 써봤는데 그렇게 하면 position이 먹게 되고 초록색동그라미(span)의 위치 잡기가 애매해서 sr-only를 빼버리고 title로 대체하였다.

---

## flex 정렬

> 1. display:flex로 정렬을 하니 옆으로만 계속 넘치듯이 정렬이 돼서 flex-wrap: wrap을 주어서 2줄로 만들었다.
> 2. 선생님 시안에는 2번째 줄과 1번쨰 줄이 순서가 바뀐거같아서 flex-wrap: wrap-reverse로 수정해서 순서를 바꿨다.
> 3. #section02 ul li에 width: calc(100% / 4 - 10px / 4)는 display:flex만으로는 딱 맞는 두줄과 이미지 사이의 간격이 잘 나오지 않아서 추가하게 되었다.

---

## 그외

> 1. section태그에 id로 setion01, section02를 준건 html 한 페이지에서 작업하는데 공통으로 들어가는거 말고 css가 다르게 작업되는 부분이 있어서 id를 추가하게 되었다.
