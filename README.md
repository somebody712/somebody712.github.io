# somebody712.github.io

배운 것과 한 일을 정리하는 Markdown 블로그입니다.

공개 주소: <https://somebody712.github.io/>

## 글 올리기

1. 저장소의 `_posts` 폴더를 엽니다.
2. **Add file → Upload files**를 눌러 `.md` 파일을 올립니다.
3. 파일 이름은 `YYYY-MM-DD-title.md` 형식으로 만듭니다.
4. `main` 브랜치에 Commit하면 자동으로 게시됩니다.

`POST_TEMPLATE.md`를 복사해 사용할 수 있습니다.

```md
---
title: "글 제목"
description: "글에 대한 짧은 설명"
category: "개발"
category_slug: development
---

## 소제목

본문을 작성합니다.
```

## 카테고리 값

| 카테고리 | `category` | `category_slug` |
| --- | --- | --- |
| 개발 | 개발 | `development` |
| CTF / Wargame | CTF / Wargame | `ctf-wargame` |
| BugbBounty | BugbBounty | `bugbounty` |
| 블로그 / 기술문서 | 블로그 / 기술문서 | `blog-docs` |
| 논문 / 컨퍼런스 | 논문 / 컨퍼런스 | `papers-conferences` |
| 공모전 / 자격증 | 공모전 / 자격증 | `contests-certifications` |

`category_slug` 값에 따라 각 카테고리 페이지에 글이 표시됩니다.
