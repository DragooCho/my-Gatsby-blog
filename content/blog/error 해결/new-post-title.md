---
title: node-sass/vendor 에러
date: 2021-01-23 00:01:36
category: error 해결
thumbnail: { thumbnailSrc }
draft: false
---

개인 프로젝트 진행중에 코드수정을 위해    
node_modules 디렉토리를 삭제하고 다시 패키지들을 설치한뒤      
npm start를 터미널로 실행했지만 node_modules/node-sass/vendor란 오류가 발생 했었습니다.    
    
        

어찌저찌 구글링 하다보니 원인은 node_modules/node-sass/vendor 디렉토리가 존재하지 않아서    
node-sass의 scripts/install.js를 실행을 못 한거였습니다.    
    
        

저의 경우에는 수동으로 node-sass의 스크립트를 실행하는걸로 해결 할 수 있었습니다.    




```````````````
$ node node_modules/node-sass/scripts/install.js
````````````````    

        

[출처: https://wonism.github.io/node-sass-vendor/ ](https://wonism.github.io/node-sass-vendor "wonism.github.io")