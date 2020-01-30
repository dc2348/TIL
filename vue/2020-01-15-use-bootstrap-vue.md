---
layout: post
title:  "Vue 프로젝트에 Bootstrap 사용하기"
date:   2020-01-16 15:00:00 +0900
categories: blog
---

# 반응형 뷰포트 메타 태그(Responsive meta tag)
```
<meta name="viewport" content="width=device-width, initial-scale=1, shrink-to-fit=no">
```
- `<head>` 태그 안에 추가하기


# CSS box-sizing
```
.selector-for-some-widget {
  box-sizing: content-box;
}
```

# Using module bundlers
###### install BootstrapVue and Bootstrap 
```
# With npm
npm install vue bootstrap-vue bootstrap
```

###### register BootstrapVue in your app entry point
```
// App.vue

import Vue from 'vue'
import { BootstrapVue, IconsPlugin } from 'bootstrap-vue'

// Install BootstrapVue
Vue.use(BootstrapVue)
// Optionally install the BootstrapVue icon components plugin
Vue.use(IconsPlugin)
```

###### import Bootstrap and BootstrapVue css files:
```
// App.vue
import 'bootstrap/dist/css/bootstrap.css'
import 'bootstrap-vue/dist/bootstrap-vue.css'
```

###### require global Vue reference
```
// App.vue
import Vue from 'vue'
```


<br>

### :bookmark_tabs: 참조(references)
https://bootstrap-vue.js.org/docs/