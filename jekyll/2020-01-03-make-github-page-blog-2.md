---
layout: post
title:  "블로그 만들기 - GitHub Pages란? Jekyll이란?"
date:   2020-01-03 16:00:00 +0900
categories: blog
---

블로그를 생성하기 전에 블로그를 운영에 사용할 GitHub Pages와 Jekyll 두 개념에 대해 간략히 정리해 보았다.
<br>

# :gem: GitHub Pages란?
GitHub Pages는 GitHub의 저장소에서 HTML, CSS 및 JavaScript 등의 파일을 직접 가져와서 빌드 프로세스를 통해 파일을 실행하고 웹 사이트를 게시하는 정적 사이트 호스팅 서비스이다.
별도의 도메인을 생성하지 않아도 GitHub의 github.io 도메인에서 사이트를 호스팅 할 수 있다. 즉, http://username.github.com 형태의 고유한 내 도메인을 무료로 운영할 수 있는 것이다.
<br>

# :gem: Jekyll이란?
Jekyll(지킬)은 정적 사이트 생성기이다. 간단히 말해서 마크다운 같은 형태의 텍스트 파일로 문서를 작성하면 그 문서를 웹 사이트 형태로 변환해주는 것이다. 즉, 우리는 HTML과 같은 복잡한 구조가 아닌 단순한 텍스트 문서 작성만으로도 웹 사이트를 만들 수 있는 것이다.

- Jekyll의 동작원리
    - 정적 사이트 생성기
    - 텍스트(마크다운) 파일로 컨텐츠를 작성하고, 폴더로 그 파일들을 정리한다.
    - Liquid 기능이 추가된 HTML 템플릿을 사용해 사이트의 모양을 만든다.
    - 자동으로 내용물과 템플릿들을 함께 합쳐서, 어떤 서버에서도 올바르게 작동하는, 완전한 정적 웹사이트를 생성한다.
<br>

# :gem: GitHub Pages에서의 Jekyll
- Jekyll은 GitHub Pages의 내부 엔진이다. 따라서 GitHub 서버에서 Jekyll을 이용하여 간편하게 페이지, 블로그, 웹사이트를 무료로 호스팅 할 수 있다.