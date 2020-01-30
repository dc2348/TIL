---
layout: post
title:  "블로그 만들기 - Github Pages로 웹호스팅하기"
date:   2020-01-03 17:00:00 +0900
categories: blog
---

이전 포스팅에서 로컬 컴퓨터에서만 확인 가능한 로컬 서버를 이용한 블로그를 확인해보았다. 이번 포스팅에서는 GitHub Pages를 이용하여 실제로 웹호스팅이 되는 블로그를 등록해볼 예정이다.



# :gem: Github에 블로그용 repository 생성하기

GitHub Pages에 웹호스팅을 하기 위해서는 Github에 블로그 용 repository가 하나 존재해야 한다. 
GitHub Pages가 웹호스팅하는 기본 repository 이름은 \<username\>.github.io이다. (여기서 username은 본인 GitHub ID를 의미한다)
따라서, Name이 \<username\>.github.io인 repository를 생성해야한다. 그럼 GitHub Pages가 https://\<username\>.github.io 주소를 웹호스팅 주소(블로그 주소)로 사용하게 된다.

- :bulb: 준비물
    - GitHub 계정
    - Git 로컬 설치

## :ring: \<username\>.github.io 형식의 Git Repository 생성
- GitHub 메인페이지에서 Repositories 탭을 클릭하여 이동한다.
- New 버튼을 클릭하여 신규 repository 생성 화면으로 이동한다.
    - Repository name에 \<username\>.github.io를 입력한다.(여기서 \<username\>은 본인 GitHub ID를 의미한다)
        - ex) dc2348.github.io (dc2348은 내 ID이다.)
    - GitHub 무료 계정이면 Public을 선택한다.(무료 계정은 Private Repository에 대한 GitHub Pages 서비스를 제공하지 않는다)
    - 이전 포스팅에서 생성해 놓은 프로젝트를 사용할 것이기 때문에, README 파일, .gitignore, license 등 초기 생성 파일들은 모두 선택하지 않는다.
![2020-01-03-createRepository-1]({{site.baseurl}}/assets/images/2020-01-03-createRepository-1.jpg)

<br>

# :gem: repository에 프로젝트 commit 하기
이제 생성한 레파지토리에 생성해두었던 블로그 프로젝트를 올려볼 것이다. cmd를 열어 아래 명령어들을 실행한다.(username은 자신의 github 계정)

- `jekyll-website`를 `username.github.io`로 이름 변경하기
    - `jekyll-website` 상위 폴더로 이동
    - `ren jekyll-website username.github.io`
- 레파지토리에 commit 하기
    - 프로젝트 안으로 경로이동
        - `cd username.github.io`
    - Git 초기화, 커밋, 푸시
        - `git init`
        - `git add .`
        - `git commit -m "FEAT:Add project"`
        - `git remote add origin https://github.com/username/username.github.io.git`
        - `git push -u origin master`

- http://dc2348.github.io 로 접속
    - 내 도메인 접속시, 블로그가 정상 노출됨
    ![2020-01-03-createRepository-1]({{site.baseurl}}/assets/images/2020-01-03-createRepository-2.jpg)


