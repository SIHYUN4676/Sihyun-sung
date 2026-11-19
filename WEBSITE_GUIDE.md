# SIHYEON. — Personal Index

`index.html`을 더블클릭해 브라우저에서 열면 됩니다. 설치나 서버가 필요 없으며, 인터넷 없이도 작동합니다.

## 사진 넣기

1. `assets` 폴더에 본인의 이미지 파일을 넣습니다.
2. `index.html` 하단의 `siteConfig`를 찾습니다.
3. 해당 값을 다음처럼 변경합니다. 실제 확장자와 파일명에 맞춰 입력하세요.

```js
portrait: 'assets/portrait.jpg',
moisilCover: 'assets/moisil-cover.jpg',
supportTable: 'assets/support-table.jpg',
```

이미지 파일을 읽을 수 없으면 기존 그래픽이 유지됩니다. 현재 그래픽은 직접 만든 교체용 표지이며 실제 인물 사진이나 완성된 프로젝트 결과물이 아닙니다. 인물 사진은 세로형, MOISIL은 가로형, SUPPORT TABLE은 세로형을 권장합니다. 잘리는 부분은 CSS의 `.asset-image`에서 `object-position: center 30%;` 같은 값으로 조정할 수 있습니다.

## 연락처·문구·색상 수정

- `siteConfig.email`에 실제 이메일을, `instagram`과 `github`에 `https://`로 시작하는 전체 주소를 입력합니다. 입력된 항목만 실제 링크로 표시됩니다.
- 소개는 `id="about"`, 관심사는 `id="interests"`, 프로젝트는 `id="work"` 부분을 수정합니다.
- 진행 상태는 각 프로젝트의 `class="status"` 문구를 수정합니다.
- 맨 위 CSS의 `:root`에서 색상을 변경합니다.
- 외부 폰트·이미지·라이브러리를 사용하지 않습니다. 영문 제목은 운영체제에 설치된 Impact 또는 대체 글꼴로 표시되어 기기마다 모양이 조금 다를 수 있습니다.

홈페이지를 다른 사람에게 전달할 때에는 `index.html`과 `assets` 폴더를 함께 전달하세요. 온라인 공개는 별도로 진행하면 됩니다.
