# hyungbin77.github.io

박형빈의 포트폴리오 사이트. [https://hyungbin77.github.io](https://hyungbin77.github.io)

통계학 석사 수료 이력과 IT/AI 직무 지원용 프로젝트를 함께 담는 것을 목표로,
[Academic Pages](https://github.com/academicpages/academicpages.github.io) 템플릿에서
학계 전용 요소(강의 이력, 강연 지도 등)를 덜어내고 프로젝트 중심으로 재구성했습니다.

## 사이트 구조

| 경로 | 내용 | 소스 |
| --- | --- | --- |
| `/` | 소개 · 기술 스택 · 대표 프로젝트 | `_pages/about.md` |
| `/projects/` | 프로젝트 목록 (메인) | `_pages/projects.html` + `_portfolio/` |
| `/research/` | 논문 · 학회 발표 | `_pages/research.html` + `_publications/` |
| `/blog/` | 학습 기록 | `_pages/blog.html` + `_posts/` |
| `/resume/` | 이력서 한 장 요약 | `_pages/resume.md` |

## 콘텐츠 추가하기

각 디렉토리의 `_` 로 시작하는 예시 파일을 복사해서 새 이름으로 저장하면 됩니다.
`_` 로 시작하는 파일은 Jekyll이 무시하므로 사이트에 표시되지 않습니다.

```
_portfolio/_example-project.md   →  _portfolio/추천시스템-개선.md
_publications/_example-paper.md  →  _publications/2025-11-01-논문제목.md
_posts/_example-post.md          →  _posts/2026-01-15-글제목.md
```

- **프로젝트** — `date` 를 반드시 넣으세요. 목록이 최신순으로 정렬됩니다.
- **연구** — `category` 를 `journal` 또는 `conference` 로 지정하면 Research 페이지에서 자동 분류됩니다.
- **PDF · 첨부파일** — `files/` 에 올리면 `https://hyungbin77.github.io/files/파일명` 으로 접근됩니다.
- **이미지** — `images/` 에 올리고 `/images/파일명` 으로 참조합니다.

## 설정

주요 설정은 모두 `_config.yml` 에 있습니다.

| 항목 | 설명 |
| --- | --- |
| `site_theme` | `default`, `air`, `sunrise`, `mint`, `dirt`, `contrast` 중 선택 |
| `author.*` | 왼쪽 사이드바에 표시되는 프로필과 링크. 값이 비면 해당 아이콘이 숨겨집니다 |
| `resume_pdf` | PDF 이력서 경로. 값을 넣으면 이력서 페이지에 다운로드 버튼이 생깁니다 |
| `publication_category` | Research 페이지의 섹션 구분 |

헤더 메뉴 순서는 `_data/navigation.yml` 에서 바꿉니다.

## 로컬에서 확인하기

```bash
bundle install
bundle exec jekyll serve --livereload
# http://localhost:4000
```

Docker를 쓰는 경우:

```bash
docker compose up
```

## 라이선스

템플릿은 MIT 라이선스를 따릅니다 (`LICENSE` 참고).
사이트에 담긴 글·프로젝트 내용의 저작권은 작성자에게 있습니다.
