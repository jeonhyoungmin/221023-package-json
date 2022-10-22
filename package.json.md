{
  "name": "221023-package-json", // 프로젝트 이름입니다.
  "version": "1.0.0", // 버전 정보 입니다.
  "description": "프로젝트의 설명을 작성하는 자리입니다.",
  "main": "index.js", // entry point 실행할 때 첫 번째로 실행할 파일을 이야기합니다.
  "scripts": {
    // "scripts" 키에는 원하는 동작 명령을 미리 설정 할 수 있다.
    // 아래의 "example" 키는 임의로 작성한 커스텀 명령으로, "" 쌍따옴표 안에는 명령 인터페이스에서 글자를 출력하는 간단한 명령이다.
    // 해당 명령을 실행시키고자 한다면,
    // npm run example <-- 이라는 방식으로 실행 할 수 있다.
    "example" : "echo \" hello \" ",

    "test": "echo \"Error: no test specified\" && exit 1"
  },
  "author": "작성자 혹은 저작권자의 데이터를 작성하는 자리 입니다.",
  "license": "ISC",
  // 개발을 위한 패키지(소프트웨어) 의존 항목 : "devDependencies"
  // 프로젝트 내에서는 활용하지만, 동작할 때는 전혀 사용하지 않는다.
  "devDependencies": {
    "@babel/cli": "^7.19.3",
    "@babel/core": "^7.19.3",
    "@babel/node": "^7.19.1",
    "@babel/preset-env": "^7.19.4"
  },
  // 배포를 위한 패키지(라이브러리 등) 의존 항목 : "dependencies"
  // '보여질' 예정인 코드들의 묶음으로 판단 할 수 있다.
  // 개발자가 한 땀 한 땀 작성한 모듈의 집합이다.
  "dependencies": {
    "react": "^18.2.0"
  },
  // 프로젝트 모듈 방식 설정, commonJS vs moduleJS
  "type": "module"
}