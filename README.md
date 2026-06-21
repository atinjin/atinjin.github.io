# atinjin.github.io

Personal blog powered by [Jekyll](https://jekyllrb.com/) + [Chirpy](https://github.com/cotes2020/jekyll-theme-chirpy).

## 새 글 작성

`_posts/YYYY-MM-DD-title.md` 파일을 만들고 아래 frontmatter로 시작합니다:

```yaml
---
title: "글 제목"
date: YYYY-MM-DD HH:MM:SS +0900
categories: [카테고리1, 카테고리2]
tags: [태그1, 태그2]
description: "한 줄 설명"
---
```

`main` 브랜치에 push하면 GitHub Actions가 자동으로 빌드·배포합니다.
