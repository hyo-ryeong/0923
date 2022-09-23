# 0923

9 dom요소 추가, 삭제 하는 법

//첫번째 ul이 선택된다.
const parentEl = document.getElementsByTagName('ul')[0];
  console.log(parentEl);

  const removeEl = document.getElementsByTagName('li')[2];
  console.log(removeEl);

// removechild를 이용해서 지워주기 
  parentEl.removeChild(removeEl);

//문서 객체 (html tag)li를 생성
  const newEl = document.createElement('li'); 
  const newText = document.createTextNode('녹차 아이스크림');
  console.log(newText);

//newEl에 newText를 넣어준다.
//A.appendChild(B) - 노드A에 노드B를 삽입해서 자식요소로 만든다.
  newEl.appendChild(newText); 
  parentEl.appendChild(newEl);
  console.log(newEl);
  

  parentEl.appendChild(newEl);
  parentEl.appendChild("<li>내일 뚱보집</li>");
  
  //A.append(B) - A요소의 내부 끝 부분에 B삽입
  //A.prepend(B) - A요소의 내부 시작 부분에 B삽입
  //A.after(B) - A요소의 뒤에 B삽입
  //A.before(B) - A요소의 앞에 B삽입
