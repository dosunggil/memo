# 웹 문서 만들기

** html : 웹문서를 만드는 언어 / 웹문서의 기본골격(명사)<br>
css(cascading style sheet) : 웹문서를 보기 좋게 꾸미는 디자인표현(형용사,부사)<br>
javascript/jQuery : 프로그래밍적 요소로 사용자의 행위에 의한 동작(동사)<br><br>


### 블록 레벨 텍스트 태그
* --혼자서 한 줄을 차지하여 너비가 100% 꽉 차게 표시되는 태그

* 1)h태그: heading태그 - 제목을 표시하는 태그 ; h1~h6 
<h1>h1 : 가장큼</h1>
<h6>h6 : 가장작음</h6>

* 2)p태그: paragraph - 단락을 표시하는 태그로 줄바꿈 없이 텍스트가 한 줄로 표시됨
<p>텍스트의 길이가 브라우저 창의 너비보다 길면 자동으로 줄이 바뀐다.</p>

* 3) br태그: 줄바꿈 태그로 끝태그가 없다. <br>

* 4) hr태그(horizontal): 주제가 바뀌거나 할 때 사용하는 가로선 표시<hr>

* 5) div태그(division) : <div>영역을 나누는 태그</div>

### 인라인 레벨 텍스트 태그
* --한 줄을 차지하지 않는 태그로 화면에 표시되는 컨텐츠 만큼의 너비를 차지하는 태그

* 1) strong태그 : 텍스트를 <strong>굵게</strong> 표시하는 태그

* 2) span태그 : 텍스트의 일부만 <span style="color:red;">스타일</span> 적용

* 3.목록을 만드는 태그
ul(unordered list): 순서없는목록 
ol(ordered list): 순서있는목록  
<ul>* 메뉴1* 메뉴2* 메뉴3
</ul> --ul 의 list-style-type 은 기본이 disc 이다

<ol s* rt="3" type="A">
	1* 2* 3
</ol> --ol의 list-style-type 은 기본이 deciaml(정수)이다

* 4. 표를 만드는 태그
table태그, tr태그(table row), td태그(table data)
행/열로 이루어진 표의 형태를 만들때 사용하는 태그
tr: 행에 해당하는 태그
td: 행 내부의 열에 해당하는 셀 태그 
th:(table head): 행 내부의 제목에 해당하는 셀 태그( 가운데 정렬, 폰트 진하게 )
caption 태그 : 표에 사용하는 표 제목 표시태그
표 상단 가운데에 위치한다.
<table style="border=1;">
    <caption>회원 목록</caption>
	<tr><th>성명</th><th>전화번호</th>
	<tr><td>홍길동</td><td>01012345678</td>
	<tr><td>손흥민</td><td>11111111111</td>
	</tr>	
</table>

### 태그에 대한 꾸미기 style 지정해보기
* 인라인 스타일: 태그에 직접지정
* 내부 스타일: 헤드 태그 안에 스타일 선언하여 설정 - html문서내부에 style 태그 안에 지정하는 형태
* 외부 스타일: style만 정하는 css파일을 따로 만들어 html 문서에 연결하는 형태

### 이미지와 비디오 태그
	
* a태그 : 링크는 현재 웹 페이지에서 다른 페이지로 연결하기 위한 형태
--<a href="웹 링크 or 지정한 id">링크로 이동</a>
* <style>
a {	text-decoration: none; 언더바 삭제
	color: inherit; /* initial;*/ 폰트의 색상을 기본으로 }
</style> 
--head 부분의 스타일에서 앵커의 기본 스타일을 설정해본것    