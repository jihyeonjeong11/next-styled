https://velog.io/@danmin20/Next.js-Typescript-Styled-component-%EC%89%BD%EA%B2%8C-%EA%B5%AC%EC%B6%95%ED%95%98%EA%B8%B0

에 관련 내용이 있습니다.

NextJS 공부 및 웹 공부용으로 fork한 template입니다.

Structure

pages components hooks shared styles 

coverage test--coverage 결과물

pages auto routing되는 페이지

components 재활용 가능한 컴포넌트

shared 유틸함수 utils.ts와 enum.ts

styled.d.ts는 인터페이스 정의를 위한 파일

_app.tsx & _document.tsx 은 커스텀을 위한 파일

_app.tsx 프로바이더 및 css import

_document.tsx 는 styled-component 도입 및 font 임포트 용

작자는 classname을 BEM으로 사용한다고 한다. Block - Element - Modifier

```
.header__navigation--navi-text {
  color: red;
}
```

나머지 내용은 파일 안에 저장되어 있다.

packagejson

 "dependencies": {
    "@next/bundle-analyzer": "^10.0.7",
    "axios": "^0.21.1",
    "babel-plugin-styled-components": "^1.12.0", // styled-component 웹팩 빌드용
    "css-loader": "^5.0.2",  // 웹팩 css 로더
    "file-loader": "^6.2.0", //웹팩 file 로더
    "next": "^12.2.5",
    "query-string": "^7.0.0", //쿼리스트링
    "react": "^17.0.1",
    "react-dom": "^17.0.1",
    "react-ripples": "^2.2.1",  //물결버튼
    "react-virtualized-auto-sizer": "^1.0.4", // flatlist처럼, 뷰포트에 보이는 부분만 렌더링 해줌 // 오토사이저는 부모의 너비와 놃이를 자식에게 prop 형태로 전달함
    "react-window": "^1.8.6", // 위 virtualized의 windowing 구현하는 경량 버전
    "styled-components": "^5.2.1",
    "styled-reset": "^4.3.4" // css 기본 스타일 리셋
  },
  "devDependencies": {
    "@babel/core": "^7.13.10",
    "@babel/plugin-syntax-dynamic-import": "^7.8.3", // 코드 스플리팅에 필요하다
    "@svgr/webpack": "^5.5.0", // svg 그리기 위함
    "@testing-library/jest-dom": "^5.11.9",
    "@testing-library/react": "^11.2.5", //테스팅
    "@types/axios": "^0.14.0",
    "@types/node": "^14.14.22",
    "@types/react": "^17.0.0",
    "@types/react-dom": "^17.0.0",
    "@types/react-window": "^1.8.2",
    "@types/styled-components": "^5.1.7",
    "@typescript-eslint/eslint-plugin": "^4.14.1",
    "@typescript-eslint/eslint-plugin-tslint": "^4.14.1",
    "@typescript-eslint/parser": "^4.14.1",
    "babel-jest": "^26.6.3", // 테스트 시 바벨로 jest가 이해하는 코드로 변경해줌
    "babel-loader": "^8.2.2",
    "eslint": "^7.18.0",
    "eslint-config-airbnb-typescript": "^12.3.1",
    "eslint-config-prettier": "^8.1.0",
    "eslint-plugin-import": "^2.22.1",
    "eslint-plugin-jsx-a11y": "^6.4.1",
    "eslint-plugin-react": "^7.22.0",
    "eslint-plugin-react-hooks": "^4.2.0",
    "jest": "^26.6.3",
    "prettier": "^2.2.1",
    "typescript": "^4.1.3"
  }