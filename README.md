# ReactJS의 기본 개념인 JSX, State, Props, Routing 등에 대해 공부한다.

To do list, 영화 웹서비스 등을 React로 개발하기 전 해보는 연습이다.

# JSX 공부하기 전 React에 대해 공부한 내용 복습

React JS는 element를 생성하고 event listener를 더하는 것을 도와준다. => React JS가 interactive power를 가지고 있다.
ReactDOM import => React element들을 가져다가 HTML로 바꿔준다.

Javascript에서 createElement를 생성했는데 앞으로 React 개발자로서, createElement를 쓸 일은 없다.
React JSX에 대해 공부하기 전, 어려운 방법으로 코드를 짰다. 이해를 위해!

ReactDOM은 container element를 root div 안에 render한다. <= ReactDOM.render(container, root); <= Github 코드 확인

createElement의 인자 => 첫번째 인자: 태그, 두번째 인자: props, 세번째 인자: content
const btn = React.createElement(
"button",
{
onClick: () => console.log("im clicked"),
style: {
backgroundColor: "tomato",
},
},
"Click me"
);
=> props에서는 id, class, 색 등등 바꿀 수 있음, property object에 event listener를 등록할 수 있다! <= javascript처럼 addEventListener 할 필요 X.

{
onClick: () => console.log("im clicked"),
style: {
backgroundColor: "tomato",
},
},
=> props object

JSX 들어가기 전 어려운 방식으로 짠 ReactJS 코드에는 데이터를 업데이트 하는 state 존재X

바로 JSX 공부! 그 후 state
