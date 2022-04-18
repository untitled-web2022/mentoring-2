# CSS 기본

## 구조


### CSS 파일
```css
선택자 {
    속성-이름: 값;
    속성-이름: 값;
}

선택자2 {
    속성-이름: 값;
    속성-이름: 값;
}
```

### 인라인 스타일
```html
<tag style="스타일-이름: 값; 스타일-이름: 값;"></tag>
```


# 선택자

## 태그 선택

```html
<div>
  <section>Section</section>
  <article>Article</article>
  <section>Section 2</section>
</div>
```

```css
section {
    background-color: purple;
}
```

## 클래스 선택

```html
<div>
  <section>Section</section>
  <article>Article</article>
  <section class="purple text-white">Section 2</section>
  <section class="purple">Section 3</section>
</div>
```

```css
.purple {
    background-color: purple;
}

.text-white {
    color: white;
}
```

## ID 선택

```html
<div>
  <section>Section</section>
  <article id="article1">Article</article>
  <section class="purple text-white">Section 2</section>
  <section class="purple">Section 3</section>
</div>
```

```css
#article1 {
    border: 1px solid black;
}
```

## 자손 선택
```css
section article {
    font-family: sans-serif;
}
```
## 자식 선택
```css
section > article {
    font-family: sans-serif;
}
```

## 일반 형제 선택
```css
section ~ article {
}
```

## 인접 형제 선택
```css
section + article {
}
```







