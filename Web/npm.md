## npm 버전 업데이트
npm install -g npm

## --save, --save-dev
그냥 install 하면 ./node_modules 디렉터리에 패키지 설치를 하고 끝. --save, --save-dev 옵션은 ./package.json 업데이트를 같이해준다.<br>
어디에 패키지 정보를 추가하느냐가 다른데, --save 옵션은 dependencies object에 추가하고 --save-dev 옵션은 devDepenencies object에 추가한다.