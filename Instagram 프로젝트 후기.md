---


---

<h1 id="instagram-클론-프로젝트-후기">Instagram 클론 프로젝트 후기</h1>
<h2 id="프로젝트-소개">1. 프로젝트 소개</h2>
<iframe width="1152" height="480" src="https://www.youtube.com/embed/uHw2Q8IyFvA" allowfullscreen=""></iframe>

<p>전세계적으로 사용되는 소셜 미디어 플랫폼 중 심플하고 재사용 가능한 컴포넌트 UI로 구현된 인스타그램 Web App 클론</p>
<h3 id="목적">1) 목적</h3>
<ul>
<li>git을 통한 협업으로 실무환경 경험</li>
<li>Http 통신을 통한 JavaScript 비동기 처리 이해</li>
<li>SPA(Single Page Application) 구축 경험</li>
<li>React 컴포넌트 Life Cycle 이해</li>
</ul>
<h3 id="개발-기간">2) 개발 기간</h3>
<ul>
<li>개발 기간 : 2020/07/06 - 2020/07/17</li>
</ul>
<h3 id="구성원">3) 구성원</h3>
<ul>
<li>프론트 5명 (각자 동일한 페이지 구현)</li>
</ul>
<h2 id="기술-스택-및-구현-기능">2. 기술 스택 및 구현 기능</h2>
<h3 id="기술-스택">1) 기술 스택</h3>
<ul>
<li>React, React-Router, Fetch API, Sass, React-icons, Faker</li>
</ul>
<h3 id="협업-툴">2) 협업 툴</h3>
<ul>
<li>Git, Slack, Notion</li>
</ul>
<h3 id="구현-기능-상세-설명">3) 구현 기능 상세 설명</h3>
<p><strong>로그인</strong></p>
<ul>
<li>UI 구현</li>
<li>fetch API로 로그인 기능 비동기 처리</li>
<li>세션스토리지 사용해서 JWT 활용</li>
</ul>
<p><strong>메인 페이지</strong></p>
<ul>
<li>보다 복잡한 UI/UX React Component로 구현</li>
<li>fetch API로 메인 페이지 데이터 로딩</li>
<li>state, props, event handling 을 통해 댓글 생성, 삭제</li>
<li>‘좋아요’ 버튼 클릭 기능</li>
<li>Story Component 클릭 이벤트 발생 시 Story Modal 창 구현</li>
</ul>
<h2 id="작업순서">3. 작업순서</h2>
<ol>
<li><code>git checkout master</code>: 마스터 브랜치로 이동</li>
<li><code>git pull origin master</code>: github에 변화된 최신 코드를 받아온다</li>
<li><code>git branch feature/name</code>: 본인의 브랜치 생성</li>
<li><code>git checkout feature/name</code>: 브랜치로 이동</li>
<li><code>git merge master</code>: 마스터에서 받아온 최신 코드를 브랜치에 병합시킨다</li>
<li><code>npm install</code>: package.json dependencies 에 추가된 모듈 로컬에 다운로드</li>
<li>최대한 기능별로 쪼개서 작업하기</li>
<li>프로젝트 상위 디렉토리로 가서 <code>git add .</code> 명령어로 내가 수정한 코드를 git stage 에 올린다</li>
<li><code>git status</code>: add가 잘 되었는지 확인</li>
<li><code>git commit -m "commit message"</code>: commit message는 팀원과 상의한 후에 slack 에 공유한다</li>
<li><code>git push origin feature/name</code>: 본인 브랜치에서 작업한 내용을 원격 리포지토리에 올린다</li>
</ol>
<h2 id="기록하고-싶은-코드">4. 기록하고 싶은 코드</h2>
<p><a href="https://dream-frontend.tistory.com/392">1) map 메소드 활용하여 인스타그램 피드 반복구문 코드 간결화</a><br>
2) fetch API 활용해 백엔드와 통신하여 로그인기능 구현<br>
3) sass 이용해 반복되는 css 코드 변수에 담아 활용</p>
<h2 id="느낀점">5. 느낀점</h2>
<ol>
<li>뿌듯한 점</li>
</ol>
<p><code>처음으로 아무것도 없는 무에서 리엑트 구현</code>을 했다는 점이 매우 뿌듯하다.<br>
바닐라 자바스크립트에서 리엑트로 옮기면서 리엑트의 SPA개념과 컴포넌트 개념이 너무 헷갈릴 때도 있었지만, 내가 직접 작성했던 코드를 옮기면서 자르고 쪼개보는 시간이 있었기에 컴포넌트 개념을 더 잘 이해를 할 수 있었다.</p>
<p>그리고 <code>처음 map 함수 활용한 실질적 사례</code>이기도 했다.<br>
알고리즘을 하거나 javascript 문법 테스트 통과하기 위해 map을 써봤지,<br>
이렇게 실질적 웹사이트 구현 사례에서 사용해 본 것은 처음이었다.</p>
<p>처음에는 map함수를 어떻게 이용하지?<br>
막막하기도 했었지만, 한번 구현해보니 다른 것들도 쉽게 적용이 가능했다.<br>
게다가 한번의 코드작성으로 수백개 수만개의 동일한 화면 구현이 가능하다는 점이<br>
매우 매력적이다:)</p>
<p>또한 <code>fetch API를 이용해 로그인 기능을 구현</code>해본 것도 재미있었다.<br>
지난 fetch 세션을 들을 때에는<br>
‘header 는 뭐지? body는 뭐고 method는 무슨 차이가 있는거지?’ 하며<br>
궁금증이 남아있었는데 그 궁금증이 이번에 많이 풀렸던 것 같다.</p>
<p>그리고 body에서 JSON.stringify를 해주어야 하는 이유,<br>
서버에서 받아온 데이터를 다시 json() 형태로 변환시켜주어야 하는 이유에 대해서<br>
직접적으로 눈으로 확인 하며 알 수 있어 매우 좋은 경험이었다.</p>
<p>마지막으로는 <code>sass 라이브러리를 처음 활용</code>해 본 것이다.<br>
sass의 가장 큰 특징은 'nesting’이라 할 수 있다.<br>
그러나 공식문서를 찾아 읽어보니 그 외에도 다양한 기능들이 있었다.<br>
변수에 담기, extends, 연산 등이 그 예이다.<br>
이번에 인스타그램 클론 코딩을 하면서는 nesting기능과 변수에 담아 활용하는 기능을 사용해보았다. 확실히 부모의 클래스네임까지 일일이 적어주던 것과는 달리 편리했다.</p>
<p>기능구현과 달리 함께 <code>팀 협업으로 git을 이용</code>해본 것도 매우 유익한 경험이었다.<br>
혼자서 git을 사용하기만 했지, 팀이 함께 같은 공동의 결과물을 내놓기 위해<br>
협업 툴로 git을 이용하며 결과물을 만든 것은 처음이었다.</p>
<p>혼자서 웹사이트를 구현할 때는 내 생각대로 클래스명도 짓고 reset.css도 자유롭게 작성했었지만, 팀이 함께 공동의 결과물을 내놓으려다보니 그냥 시작할 수가 없었다.</p>
<p>함께 어떤 reset.css, common.css를 줄지 고민하고 결정해야했고,<br>
이를 통해 초기 세팅이 매우 중요하다는 것을 몸소 경험할 수 있었다.</p>
<p>그렇게 오랜시간 세밀하게 공통부분을 맞춘다고 맞추었음에도<br>
git merge 시 충돌이 나기는 했다ㅎㅎ</p>
<p>그 덕에 충돌해결방법까지 경험해볼 수 있는 시간이었다.<br>
(git pull 이후, npm install이 얼마나 중요한 과정인지 깨달았음😹)</p>
<ol start="2">
<li>아쉬운 점</li>
</ol>
<p>좀 더 <code>다양한 기능구현을 더 하지 못했던 점</code>이 아쉬웠다.<br>
예를들면,<br>
스토리 모달창이라던지 (현재 모달창 구현중…)<br>
백엔드와 통신한 피드 검색기능,<br>
자동로그인 기능 같은 것을 더 구현해보지 못했던 것이 아쉬웠다.</p>
<p>자바스크립트를 배우고, 리엑트를 함께 하다보니<br>
점점 다양한 기능구현들에 욕심이 나기 시작했다…ㅎㅎㅎ<br>
이것도 해보고 싶고 저것도 해보고 싶었다.</p>
<p>이번에는 리엑트 기초 사용경험을 다지는 시간이었다면,<br>
다음 본격적인 첫 프로젝트 때는 css 구현도, 데이터를 다루는 기능구현도<br>
좀 더 집중해서 구현해보고 싶다.</p>

