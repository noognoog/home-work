<!-- 여기에 회고 내용을 작성해주세요 -->

# css 회고

- css도 원리를 바탕으로 적용해보니 알찼다.
- 모든 속성을 다 외울 수는 없을 것 같은데, 자주 쓰는 것들은 원리를 확실히 공부하고 + 많이 써보고 익숙해져야겠다.

# avatar 과제 회고

- 블록 요소 ul>li를 두 개 이용해서 한줄씩 배치했는데, 그게 아니라 하나의 블록 요소에 8개를 넣고, 4개씩 나눠서 배치하는 방법은 flex-box를 배우고 적용해봐야겠다. 다음 주에 수업 때 배우고 써먹어봐야지.
- avatar의 상태 정보를 스크린 리더에 표시하기 위해서 아래와 같이 처리를 했는데, 제대로 한건지 잘 모르겠다. 접근성 공부를 더 해야겠다.

```html
<li>
  <img src="/src/avatars/images/face6.jpg" alt="사용자 아바타" />
  <span class="visually-hidden">활성 상태</span>
</li>
<li>
  <img src="/src/avatars/images/face7.jpg" alt="사용자 아바타" />
  <span class="visually-hidden">비활성 상태</span>
</li>
```

```css
.visually-hidden {
  position: absolute;
  width: 1px;
  height: 1px;
  margin: -1px;
  overflow: hidden;
}
```
