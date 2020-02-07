---
layout: post
title:  "Vue-CLI를 이용하여 Vue 프로젝트를 Github Pages에 호스팅하기"
date:   2020-01-15 18:00:00 +0900
categories: vue
---

# 퍼블릭 경로 설정

###### vue.config.js 파일 생성하기
- `vue.config.js` 파일은 추가적인 설정 파일이다.
- `vue.config.js` 파일을 프로젝트의 root 경로에 생성한다.
- `vue.config.js` 파일은 옴션들을 포함한 하나의 object를 export 해야한다.
```
// vue.config.js
module.exports = {
  // options...
}
```

###### publicPath 설정하기
```
module.exports = {
    publicPath: process.env.NODE_ENV === 'production'
    ? '/'
    : '/'
}
```

# 배포파일 생성하기
```
npm run build
```


```
cd dist
git init
git add -A
git commit -m "BLD:Add new version"
git push -f https://github.com/dc2348/dc2348.github.io.git master
```

<br>

### :bookmark_tabs: 참조(references)
https://cli.vuejs.org/guide/deployment.html#github-pages
https://cli.vuejs.org/config/#publicPath
https://soobakba.tistory.com/16