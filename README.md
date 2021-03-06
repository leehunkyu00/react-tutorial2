## React tutorial
React의 component 기반 예제를 기반으로 외부 라이브러리를 추가하는 예제

## step 1. git repository 만들기
### pre-work
Create repository for 'react-study' on github

### work
```
$ mkdir react-study
$ cd .\react-study\
$ git init
$ echo "# react-study" >> README.md
$ git init
$ git add .\README.md
$ git commit -m "fisrt commti"
$ git log
$ git commit --amend
$ git remote add origin https://github.com/leehunkyu00/react-study.git
$ git push -u origin master
```

.gitignore 파일 생성
node_modules 작성


## step 2. "Hello World!" with React.js

### pre-work
Visual studio code 설치


### work
```
$ npm install react react-dom
$ npm install --save-dev react-scripts
$ code .
```

package.json 수정
"scripts": {
	"start": "react-scripts start",
	"build": "react-scripts build",
	"eject": "react-scripts eject",
},

src폴더 생성후 index.js 파일 생성
```
src/index.js
// 코드 작성
mport React from 'react';
import ReactDOM from 'react-dom';

class Board extends React.Component {
    render() {
        return (
            <div>
                Hello world!!
            </div>
        )
    }
}

ReactDOM.render(
    <Board />,
    document.getElementById('root')
)
//


```
public폴더 생성  
favicon.ico 복붙  
index.html 복붙  
manifest.json 복붙


terminal에서   
$ npm start  
그리고 localhost:3000 에서 확인


## step3. index.css 적용

src/에 index.css적용학
index.js에 import 

## step4. Create a game frame

index.js 수정

## step5. Adjust props

Board의 renderSquare function에서 Square에 value 주고
index.js의 Square에 this.props적용하기 

## step6. Button의 onClick

button에서 onClick={function() { alert('click')} 을 작성한다.

## step7. React의 state에 대해서

onClick에 this.setState을 넣어본다.

## step8. this.setState와 props의 관계에 대해서

setState로 변한 값이 props에 적용되는 것을 확인한다.

## step9. X와 O의 순서에 대해서
X를 클릭한 후에 O이 클릭이 되도록 수정한다.

## step10. X와 O중 누가 승리했는지 확인한다.
승리 조건을 확인하는 function을 이용하여 확인한다.

## step11. history를 기록하고 복기한다.
history을 state로 관리한다.

## step12. 외부 library사용, css적용하는 방법
ant design의 Step을 적용시키고 X, O의 텍스트를 Icon으로 변경한다.

antd 설치  
$ npm install --save antd

https://ant.design/components/steps/  
https://ant.design/components/icon/