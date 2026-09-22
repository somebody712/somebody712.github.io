# somebody712.log

`https://somebody712.github.io/`에 게시하도록 준비한 Jekyll 기반 Markdown 블로그입니다. 홈, 글 목록, RSS, 소개 페이지와 6개 카테고리별 글 페이지가 포함되어 있습니다.

## GitHub에 게시하기

1. `somebody712` 계정에서 공개 저장소 `somebody712.github.io`를 만듭니다.
2. 이 폴더 **안의 파일과 폴더 전체**를 저장소의 `main` 브랜치 최상위에 올립니다. `.github/workflows/pages.yml`도 포함해야 합니다.
3. 저장소의 **Settings → Pages → Build and deployment → Source**를 **GitHub Actions**로 설정합니다.
4. **Actions** 탭에서 `Deploy GitHub Pages` 작업이 완료되면 `https://somebody712.github.io/`에 접속합니다. 첫 게시에는 시간이 걸릴 수 있습니다.

현재 `_config.yml`은 이 주소에 맞게 설정되어 있습니다. 다른 저장소나 도메인으로 게시할 때는 `url`과 `baseurl`을 바꿔야 합니다.

## 새 글 작성하기

`_posts`에 `YYYY-MM-DD-영문-슬러그.md` 형식의 파일을 추가합니다.

```markdown
---
layout: post
title: "새 글 제목"
description: "글을 한 문장으로 소개합니다."
category: development
---

여기에 **Markdown**으로 본문을 작성합니다.
```

`category`에는 다음 ID 중 **하나**를 입력합니다.

| 표시 이름 | 입력할 ID |
| --- | --- |
| 개발 | `development` |
| CTF/Wargame | `ctf-wargame` |
| BugbBounty | `bugbounty` |
| 블로그/기술문서 | `blog-docs` |
| 논문/컨퍼런스 | `papers-conferences` |
| 공모전/자격증 | `contests-certifications` |

카테고리 이름과 설명은 `_data/categories.yml`에서 수정할 수 있습니다. 파일명의 날짜가 게시일이며 미래 날짜의 글은 기본적으로 표시되지 않습니다. `_posts`의 시작 글은 주제별 글 작성 예시이므로 본인의 경험과 자료로 수정하거나 교체하세요.

이미지는 `assets` 폴더에 넣고 글에서 `![설명]({{ '/assets/이미지.png' | relative_url }})` 형태로 참조할 수 있습니다.

## 수정할 파일

- `_config.yml`: 사이트 제목, 소개, URL
- `about.md`: 운영자 소개
- `assets/css/style.css`: 화면 스타일
- `assets/favicon.svg`: 브라우저 아이콘

## 로컬 미리보기

Ruby와 Bundler가 설치된 환경에서 다음 명령을 실행합니다.

```bash
bundle install
bundle exec jekyll serve
```

브라우저에서 `http://localhost:4000`을 엽니다.
