# somebody712 Portfolio

`https://somebody712.github.io/`에 게시되는 한 페이지 포트폴리오입니다. 소개, 활동·경력, 프로젝트, GitHub 링크만 표시합니다. 내용이 없는 활동·경력 섹션은 자동으로 숨겨집니다.

## 내용 수정

`_data/portfolio.yml`에서 이름, 소개, GitHub 주소와 항목을 수정합니다. 경력과 활동은 `experience`, `activities` 아래에 추가합니다.

```yaml
experience:
  - period: "2024.03 — 2025.02"
    title: "회사 또는 조직"
    role: "담당 역할"
    description: "수행한 일과 결과를 구체적으로 적습니다."
    url: "https://관련-링크"

activities:
  - period: "2025"
    title: "활동 이름"
    role: "참여 역할"
    description: "활동 내용과 결과를 적습니다."
```

실제 이력만 공개하세요. 항목을 여러 개 추가하면 사이트에 자동으로 나열됩니다. 프로젝트는 같은 파일의 `projects` 목록에서 수정합니다. 색상과 간격은 `assets/css/style.css`에서 바꿀 수 있습니다.

## 게시

이 저장소의 `main` 브랜치에 변경 사항을 올리면 `.github/workflows/pages.yml`이 Jekyll 사이트를 빌드하고 GitHub Pages에 배포합니다. 배포 상태는 GitHub 저장소의 **Actions** 탭에서 확인할 수 있습니다.
