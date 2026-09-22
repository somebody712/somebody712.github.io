---
layout: post
title: "Markdown으로 블로그 글 쓰기"
description: "파일 하나로 글을 작성하고 GitHub Pages에 게시하는 방법."
category: blog-docs
---

이 블로그는 Markdown 파일을 글의 원본으로 사용합니다. 저장소의 `_posts` 폴더에 파일을 추가하면 Jekyll이 글 페이지와 목록을 생성합니다.

## 새 글 만드는 방법

1. `_posts` 폴더에 `YYYY-MM-DD-글-이름.md` 형식으로 파일을 만듭니다.
2. 파일 맨 위에 아래처럼 제목과 설명을 적습니다.
3. 그 아래부터 Markdown으로 글을 씁니다.

```yaml
---
layout: post
title: "새로운 글 제목"
description: "글을 한 문장으로 소개해 주세요."
category: development
---
```

## Markdown 예시

### 목록과 인용

- 간결하게 글을 정리할 수 있습니다.
- **굵은 글씨**, *기울임*, [링크](https://docs.github.com/pages)를 사용할 수 있습니다.

> 좋은 기록은 다시 읽을 수 있는 생각입니다.

### 코드

```javascript
const message = "안녕하세요, Markdown!";
console.log(message);
```

글의 카테고리는 여섯 가지 중 하나를 지정합니다. 사용 가능한 ID는 저장소의 `_data/categories.yml`에서 확인할 수 있습니다.
