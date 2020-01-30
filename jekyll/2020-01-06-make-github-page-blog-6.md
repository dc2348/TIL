---
layout: post
title:  "블로그 만들기 - Jekyll 블로그에서 이모지(emoji) 사용하기"
date:   2020-01-06 13:30:00 +0900
categories: blog
---

지난 포스팅에서 마크다운 파일로 글을 등록하는 내용을 이야기했었다. 그런데 마크다운 문서에 넣어둔 이모지(emoji)들이 정상적으로 변환되어 나오지 않고 그냥 텍스트 형태로 노출되었다. 찾아보니 jemoji라는 jekyll에서 사용할 수 있는 플러그인이 있었다.

<br>

# :gem: jemoji 설치하기
jekyll 프로젝트에서 jemoji 플러그인을 추가하는 방법은 간단했다.
단순히 Gemfile에 명령어 한줄을 추가해주면 된다.

- Gemfile은 프로젝트의 최상위 폴더에 위치하고 있다.
    - ![2020-01-03-createRepository-1]({{site.baseurl}}/assets/images/2020-01-06-installJemoji-1.jpg)
- Gemfile에서 명령어 추가
    - `gem 'jemoji', '~> 0.11.1'`
    - ![2020-01-03-createRepository-1]({{site.baseurl}}/assets/images/2020-01-06-installJemoji-2.jpg)

<br>

- :bulb: 참고
    - 만약 Gemfile에 위 명령어를 추가 후 tzinfo 관련 오류가 날 경우 이는 Windows에서 발생하는 오류로, Gemfile의 `gem 'tzinfo-data', platforms: [:mingw, :mswin, :x64_mingw, :jruby]` 이 부분을 주석처리하고 실행해보면 정상 실행된다. 
        - ![2020-01-03-createRepository-1]({{site.baseurl}}/assets/images/2020-01-06-installJemoji-3.jpg)

<br>

## :bookmark_tabs: 참조(references)
- [https://rubygems.org/gems/jemoji](https://rubygems.org/gems/jemoji), GitHub-flavored emoji plugin for Jekyll