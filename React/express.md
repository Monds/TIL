# React express 연동

2019.4.28 작성된 버전

## 1. 필요한 dependencies 설치
    yarn add express

nodemon: 서버측 코드가 수정되면 서버를 자동으로 재시작
concurrently: npm 명령어 동시 수행 가능

## 2. server/index.js
    const express = require('express');
    const path = require('path');
    const os = require('os');

    const app = express();
    const PORT = process.env.PORT || 3000;

    app.use(express.static(path.join(__dirname, '..', 'build/')));

    // if you need api routes add them here

    app.listen(PORT, function () {
      console.log(`Listening on port ${PORT}!`);
    });

## 3. npm script 수정

    ...
    "scripts": {
      "start": "node scripts/start.js",
      "build": "node scripts/build.js",
      "test": "node scripts/test.js",
      "server": "nodemon server/index.js",
      "dev": "concurrently \"yarn server\" \"yarn start\"",
    },


## 4. 테스트
개발 모드일 경우

    yarn dev
서버 모드일 경우 (배포)

    yarn build
    yarn server
