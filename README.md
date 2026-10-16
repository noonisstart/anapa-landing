# ANAPA 무료 자세관리 상담 랜딩페이지

빌드 과정 없는 정적 사이트입니다. Vercel에서 Framework Preset은 **Other**, Build Command는 비워 두면 됩니다.

## 구조

- `index.html` — 페이지 본문
- `assets/` — 이미지, Pretendard 폰트, 렌더링 런타임(`runtime.js`), React/ReactDOM 로컬 사본
- `vercel.json` — `/assets` 캐시 헤더

## 구글폼 주소 바꾸기

`index.html` 하단의 `FORM_URL` 값을 바꾸면 모든 상담 신청 버튼에 반영됩니다.

```js
const FORM_URL = "https://forms.gle/...";
```

## 로컬 미리보기

`file://`로 열면 `/assets/...` 경로가 깨지므로 간단한 로컬 서버로 확인하세요.

```
npx serve .
```
