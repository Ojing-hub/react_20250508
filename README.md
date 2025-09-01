npx create-react-app . : 현재 폴더 내에 react 생성
npm start : 서버 라이브 오픈

rafce : js에서 화살표 함수 형식으로 해당 폴더 이름의 변수 생성 명령어

> 터미널 내에 작성(package.json에서 설치/버전 확인 가능)
npm install react-router-dom
npm install gsap
npm install sass

※npm i 명령어로 node_modules과 설치된 프로그램의 버전도 최신 버전으로 확인 및 재설치

> App.js에서 작성하여 연동
import { BrowserRouter,Route,Routes } from 'react-router-dom';

const App = () => {
  return (
    <BrowserRouter>
      <Routes>
        <Route path='/' element={<Homeview />} />
      </Routes>
    </BrowserRouter>
  )
}

자식요소가 있는 컴포넌트
> 부모 컴포넌트에서 작성
const Main = ({children}) => {
  return (
    <main id='main' role='main'>
        {children}
    </main>
  )
}