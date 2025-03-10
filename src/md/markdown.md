# 마크다운 문법

# 개요

- plain text 기반의 마크업 언어.<br/>
- VScode에서 Ctrl+P+Markdown:Open Preview를 통해서 실시간으로 어떻게 작성되는지 볼 수 있다!<br/>
- 대부분의 HTML 태그를 같은 기능으로 사용 가능하다<br/>
  <br/>
  <br/>

# 제목

- html시간에서 배운 h1, h2, h3, h4, h5, h6을 #, ##, ###, ####, #####, ###### 로도 편하게 쓸 수 있다.
- 물론, heading 태그 안에 작성해도 결과는 똑같은 것 같다.
- html과는 다르게 heading을 쓰면 밑에 라인이 자동으로 추가된다.
  <br/>
  <br/>

# 텍스트 속성

- 아스터리스크 두 개씩을 사이에 넣고 텍스트를 넣으면 볼드 처리된다. **바로 이렇게**
- 아스터리스크와 텍스트는 붙여 써야하는듯하다.
- 이탤릭은 아스터리스크 한 개. _이렇게_
- 취소선(strike through)은 틸더 2개(~) ~~이렇게~~
- 이 모든 것들을 텍스트와 붙여서 써야 적용된다. 다시 말해서, ** 이렇게 띄어쓰면 적용이 안된다 **
- 참고로, 인용은 '>'를 써주고 내용을 적어주면 된다.
  > 이것이 바로 인용문이다.
  > <br/>
  > <br/>

# 하이퍼링크 & 이미지

- html에서의 a태그의 기능은 대괄호와 소괄호를 사용해서 구현할 수 있다. 대괄호 안에는 텍스트를, 소괄호 안에는 링크를 넣으면 된다.
- html 태그쓸때는 href뒤에 "" 안에 경로를 넣어야하나, 마크다운에서는 그냥 경로만 써도 된다.
- <a href="https://www.naver.com">html태그로 만든 하이퍼링크</a>
- [markdown의 괄호를 이용해 만든 하이퍼링크](https://www.naver.com)
- 이미지는 하이퍼링크만들때의 문법에 앞에 느낌표만 붙여주면 된다.<br/>
- ![이미지 예시](../assets/images/chiikawa.jpg)
  <br/>
  <br/>
- 물론 img 태그를 이용해도 된다
- <img src="../assets/images/chiikawa.jpg" alt="공부하고 있는 치이카와">
  <br/>
  <br/>

# 표 만들기

- '|' 기호를 이용해서 표를 만들 수 있다.
- '-'를 이용해서 구분선을 넣어주고, |를 이용해서 셀 영역을 구분해서 만들면 된다.

| 제목 1 | 제목 2 | 제목 3 |
| ------ | ------ | ------ |
| 내용 1 | 내용 2 | 내용 3 |
| 행 2   | 행 2   | 행 2   |

<br/>
- 근데 이렇게 정렬 안 된 채로 보면 불편하니까 정렬을 해줍시다.
- 정렬은 셀을 구분하는 '|'옆에 콜론을 붙여주면 된다. 가운데 정렬은 양 옆에 붙여주면 된다
- 순서대로 왼쪽 정렬, 오른쪽 정렬, 양쪽 정렬이다.

| 제목 1 | 제목 2 | 제목 3 |
| :----- | -----: | :----: |
| 내용 1 | 내용 2 | 내용 3 |
| 행 2   |   행 2 |  행 2  |

<br/>
<br/>

# 코드 보여주기

- 코드는 백틱(`)을 이용해서 보여줄 수 있다.
- 어떤 언어인지는 백틱 뒤에 명시해주면 알아서 highlight된다.

```python
print("this is a python code block example")
```

<br/>
<br/>

# 기타 알아두면 좋을 만한 문법

## 수식 작성

- 수식은 기본적으로 LaTeX 문법을 따른다.
- 요런 식으로 써주면 된다.
  $$
  \frac{n!}{k!(n-k)!} = \binom{n}{k}
  $$
- $E = mc^2$
-
