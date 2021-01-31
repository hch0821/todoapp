# todoapp

## 기술 스택

`NodeJS` `Expres.js` `MongoDB` `Bootstrap`, `EJS`

## 개발환경 구성

<details>
<summary> 펼치기/숨기기 </summary>
- [Node.js](https://nodejs.org/ko/)
- Express
  ```bash
  npm init
  npm i express
  ```
- [ES 모듈 사용 가능하게 하기](https://www.daleseo.com/js-node-es-modules/)

```js
// package.json 최상위에 코드 추가
"type": "module"
```

- Nodeman (파일 변경 감지)

  ```bash
  sudo npm i -g nodemon
  nodemon server.js
  ```

- [Bootstrap 4.6](https://getbootstrap.com/)

- bodyparser (Request body parser)

  ```bash
  npm i body-parser
  ```

- MongoDB
- https://cloud.mongodb.com/ 에서 클러스터 생성 > Database Access, Network Access 설정, URL 복사
  ```bash
  npm i mongodb
  ```
- Clusters > Connect > Connect your Application 선택 > code 복사 > 프로젝트에 붙여넣기
- Clusters > Collection 추가

- [.env 이용하여 환경 변수 설정](https://medium.com/@megastar98/using-environment-variables-in-your-node-project-66f284cd9fe6)

  ```bash
  npm i dotenv
  ```

- EJS(html view engine)
  ```bash
  npm i ejs
  ```
- html에서 지원하지 않는 PUT, DELETE 요청을 받을 수 있도록 모듈

  ```bash
  npm i method-override
  ```

  - server.js에 다음 코드 추가

  ```js
  import methodOverride from 'method-override';
  app.use(methodOverride('_method'));
  ```

- 로그인 인증 관련 모듈
  ```bash
  npm i passport passport-local express-session bcrypt
  ```
  </details>

## 배포

### 배포된 서버

https://todo-app-303417.du.r.appspot.com

### 배포 방법

Google Cloud Platform (무료 플랜)
