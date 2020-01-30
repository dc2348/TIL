---
layout: post
title:  "블로그 만들기 - Jekyll 블로그에서 Markdown으로 포스팅하기"
date:   2020-01-06 13:00:00 +0900
categories: blog
---

지난 포스팅에서 Jekyll 블로그를 생성하고 웹호스팅하는 방법까지 알아보았었다. 이번에는 markdown 파일로 글을 등록하는 방법을 소개한다.

<br>

# :gem: jekyll 폴더 구조 및 마크다운
우리가 생성한 블로그 프로젝트에 보면 _posts라는 폴더가 존재한다.
<br> ![2020-01-06-post-1]({{site.baseurl}}/assets/images/2020-01-06-post-1.jpg)

그리고 그 아래에는 2020-01-03-welcome-to-jekyll.markdown이라는 파일이 들어있다.
<br> ![2020-01-06-post-2]({{site.baseurl}}/assets/images/2020-01-06-post-2.jpg)

이게 바로 우리 블로그 첫 화면에 등록되어있는 `Welcome to Jekyll!`이라는 글의 원본 파일이다.
<br> ![2020-01-06-post-3]({{site.baseurl}}/assets/images/2020-01-06-post-3.jpg)

<br>

# :gem: 블로그에 새 글 추가하기
새 글을 추가하기 위해서는 마찬가지로 _posts 파일아래애 markdown 형식의 문서를 만들어 등록해주면 된다. <br>
![2020-01-06-post-4]({{site.baseurl}}/assets/images/2020-01-06-post-4.jpg)
- 위의 4개 파일이 신규로 추가한 파일들이다.
- 파일 이름은 주로 `"날짜(YYYY-MM_DD) + 파일명 + .md"` 형식을 갖는다
    - md는 markdown의 약자로 주로 간편하게 .md로 사용한다.
- 저장 후 다시 로컬 서버에 접속해보면 post들이 추가되어 있다.
    ![2020-01-06-post-5]({{site.baseurl}}/assets/images/2020-01-06-post-5.jpg)