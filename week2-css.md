# CSS 기본 - 가상 선택자, 속성


## 의사 선택자(pseudo-selector)
```css
section:active {
    
}
```

### active
- 해당 요소를 클릭하고 있을 때
### hover
- 해당 요소 위에 마우스를 올렸을 때

### first-child
- 실제 선택자 부분의 부모 중 첫번째 자식만 선택

### nth-child(123)




## 속성

### margin, padding

margin - border를 기준으로 바깥쪽의 공간을 만들어줌
padding - border를 기준으로 안쪽의 공간을 만들어줌

margin 은 음수로 설정이 가능하지만 padding은 불가능하다!!

### border
요소의 윤곽선을 만들어줌, border-width, border-style, border-color 로 축약 가능
border-radius 로 모서리를 둥글게 만들 수 있다.

```css
* {
    border-width: 4px; // margin, padding과 동일한 형태로 사용 가능
    border-left-width: 8px;
    border-left-style: dashed; // 특정 방향에 대한 설정도 가능
    
}
```

### display

가장 중요한 두가지 속성
- block: 해당 태그를 div처럼 각각의 공간을 가지도록 취급(한줄에 하나씩)
- inline: 해당 태그를 span처럼 텍스트처럼 취급(한줄에 여러개도 가능)

- inline은 width, height 로 크기 변경 불가, 컨텐츠에 맞게 크기 조정
- inline-block: 바깥은 inline 처럼 취급, 안쪽(컨텐츠) block 취급을 함
-> 크기 조정이 가능하다

### background
background-attachment: 


### position

#### absolute
- 절대좌표
- left, right, top, bottom 값으로 설정 가능
- left, right 와 top, bottom 동시에 있을 경우, left/top 이 우선
- 각 방향을 기준으로 얼마나 떨어져 있는지를 크기로 표현 left: 100px; 이라면 왼쪽으로부터 100px

### relative
- 상대적
- 다른 요소와의 위치를 기준으로 자동으로 정렬해 줍니다.
- 아무것도 안적은거랑 position: relative 를 적은거랑 똑같습니다.

### fixed
- 스크롤과 상관 없이 항상 동일한 위치를 유지합니다

### sticky
- 요소가 화면 밖을 나가기 전 까지는 원 위치를 유지하지만 밖으로 나가려고 하면 fixed처럼 스크롤과 관계 없이 마지막 위치로 배치됩니다.
