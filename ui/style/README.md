# 스타일 지정

### 스타일 종류
<table>
	<tr><th>인라인 스타일</th>
		<td>태그에 직접 스타일을 지정하는 형태</td>
		<td><태그 style='속성명1:값; 속성명2:값;'></td>
	</tr>
	<tr><th>내부 스타일</th>
		<td>head 태그 안에 style태그를 선언하고,<br> style 태그 내부에 스타일을 지정하는 형태</td>
		<td>&ltstyle&gt 선택자(태그이름) {속성명1:값; 속성명2:값;}&lt/style&gt</td>
	</tr>
	<tr><th>외부 스타일</th>
		<td>외부파일에 스타일을 &nbsp;&nbsp;&nbsp; 지정하고,<br> head태그 안에 외부파일을 연결하는 link를 선언한다</td>
		<td>&ltlink rel="stylesheet" href="스타일파일 경로"&gt</td>
	</tr>
</table><br><br><hr>
<table>
	<tr><th>text-align</th>
		<td>태그의 위치를 지정하는 스타일</td>



</table>


### 선택자 알아보기

* <table>
	<colgroup>
		<col width="300px">
		<col width="200px">
		<col>
	</colgroup>
	<thead>
		<tr><th>구분</th>
			<th>표현</th>
			<th>설명</th>
		</tr>
	</thead>
	<tbody>
		<tr><th>전체선택자</th>
			<td>*</td>
			<td>모든 태그에 적용</td>
		</tr>
		<tr><th>태그선택자</th>
			<td>태그명</td>
			<td>해당 태그에 적용</td>
		<tr>
		<tr><th>id 선택자</th>
			<td>#id명</td>
			<td>해당 <span class="eng">id</span>가 지정된 태그에 적용 (예 : 텍스트크기확인)
				<br>:유일해야 한다</td>
		<tr>
		<tr><th>class 선택자</th>
			<td>.class명</td>
			<td>해당 <span class="eng">class</span>가 지정된 태그에 적용
				<br>:동일한 클래스를 여러 태그에 선언가능</td>
		<tr>
		<tr><th>자식 선택자</th>
			<td>선택자 > 자식선택자</td>
			<td>선택자의 바로 아래 위치한 자식선택자에만 적용<br> (자손선택자는 적용x)</td>
		<tr>
		<tr><th>자손 선택자</th>
			<td>선택자 자식선택자</td>
			<td>선택자의 아래 위치한 모든 자손선택자에 적용<br> (자식선택자 포함)</td>
		<tr>
		<tr><th>속성선택자</th>
			<td>선택자[속성=값]</td>
			<td>속성이 특정 값을 갖는 선택자에 적용 (../3021/join.html 확인)</td>
		<tr>
	</tbody>
</table><br>
<span id="text">텍스트 크기 확인</span>
<p id="content">전체선택자를 통해서 <span class="eng">html</span> 파일내의 모든 태그에 대해 동일한 스타일을 적용할 수 있다.</p>


### 텍스트 관련 스타일

* 
style>

@import url('https://fonts.googleapis.com/css2?family=Noto+Sans+KR:wght@300&display=swap');
body { font-family: 'Noto Sans KR', sans-serif; }
#shadow {text-shadow: 2px 1px 2px red; } /* 좌우상하/번짐의정도/색상*/
#kcgi {width: 150px; border: 1px solid;/*눈으로 영역 확인하기 위한 테두리*/
/*     white-space: normal; */
/*     white-space: pre; */
/*  	   white-space: pre-wrap; */
/*  	   white-space: pre-line; */
 	   white-space: nowrap; 
	   overflow: hidden; /*영역을 벗어나면 안보이게*/
	   text-overflow: ellipsis;  /*말줄임표시*/
	   }
	   
/* 말줄임 되어진 태그의 내용에 대해 마우스를 갖다 올렸을때 보이게 처리 */
#kcgi:hover {overflow:visible;}

/* white-space: normal   = 공백은 한개로 합쳐져 보인다.
						   여러줄도 병합되어 한 줄로 합쳐짐. 
						   자동으로 줄 바꿈.
		
				nowrap   = 공백은 한개로 합쳐져 보인다.
						   여러줄도 병합되어 한줄로 합쳐짐.								 
						   줄바꿈 안됨.
		
				pre      = 공백 유지됨.
						   여러 줄 유지됨.
						   줄바꿈 안됨. 
		
				pre-wrap = 공백 유지됨.
						   여러 줄 유지됨.
						   자동으로 줄 바꿈

				pre-line = 공백은 한개로 합쳐져 보인다
						   여러 줄 유지됨.
						   자동으로 줄 바꿈
*/

table th, td {text-align: left; /*padding: 0 10px;*/ text-indent:20px;}
th, td {padding:5px 0; line-height:30px;}
ul {list-style-type: circle; border: 1px solid;}

ul#menu { display:inline-block;/*인라인으로 하면 리스트 스타일 타입이 none으로 된다*/
		   width: 200px;}
/*ul : display가 block = 너비가 100% (block 레벨이니까)
	   display: inline-block = 너비를 지정해서 적용시킬 수 있다.
	   block 이 아니면 list-style-type이 none으로 된다
	   */	 
.bg {width:300px; height:200px; border: solid 1px #232;
		margin: 20px auto; }
 
 #bg1 {background-image: url("../images/cat1.jpg"); 
 	   	background-size: 100px 50px; background-repeat: no-repeat;
 	   	background-position: center;}
 #bg2 {background-image: url("../images/cat1.jpg"); }
 #bg3 {background-image: url("../images/logo2.jpg");
  		background-size: cover; }  /*cover는 이미지를 확대나 축소하여 꽉 채움*/
 
 footer {font-size: 12px;}
 address {font-style:inherit;}
 
 
/style

* 색상과 배경관련 스타일

<ul>
	<li>background-image: 배경이미지를 url로 지정한다.</li>
	<li>background-size: 배경이미지의 크기 지정</li>
	<li>background-repeat: 배경이미지의 반복 여부</li>
	<li>background-position: 배경이미지의 위치</li>
</ul>

<!-- <div id="bg1" class="bg">
</div>

<div id="bg2" class="bg">
</div>

<div id="bg3" class="bg">
</div> --> 스타일 안에서 아이디 지정을 해서 이렇게 배경이미지를 지정할 수 있다

* 문단 스타일

<p>텍스트로 된 문단의 정렬(align), 들여쓰기(indent), 줄간격(height) 등에 대한 스타일</p>
<table>
	<colgroup>
		<col width="100px">
		<col width="200px">
	</colgroup>
	<caption>기본정보</caption>
	<tr><th>아이디</th>
		<td>hong</td>
	</tr>
	<tr><th>성명</th>
		<td>홍길동</td>
	</tr>
	<tr><th>연락처</th>
		<td>010-3673-2216</td>
	</tr>	
	<tr><th>특징</th>
		<td>소설 '홍길동전'의 주인공으로 초능력을 부리는 인물로 코리안 
		슈퍼히어로의 시초이자 대표 격이다.</td>
	</tr>	
</table><hr>


* 텍스트 관련 스타일
<p>글꼴 자체가 아닌 글자들(텍스트)에 대한 스타일</p>

<ul>
	<li>text-shadow : 그림자 효과</li>
	<li>white-space : 공백문자(스페이스바), 탭, 줄바꿈에 대한 처리</li>
	<li></li>
	<li></li>
	<li></li>
	<li></li>
</ul>
<p id="shadow">텍스트에 그림자 효과 주기</p>
<p id="kcgi">KCGI가 주주 제안한 사외이사 선임과
정관 일부        변경 안건이 
모두 주주총회에서 
부결됐기
      때문이다.</p>
<hr>
<h3>글꼴 관련 스타일</h3>
<p>font(글꼴) : 크기, 굵기, 글꼴형태를 지정할 수 있다.</p>
<table>
	<tr><th>font-weight</th>
		<td>폰트의 굵기: normal(default), bold(굵게),<br> border(가지고 있는 폰트 중 더 두꺼운 폰트 적용)</td>
	</tr>
	<tr><th>font-style</th>
		<td>기울기: normal(default), italic</td>
	</tr>
	<tr><th>font-size</th>
		<td>폰트의 크기: 보통 px로 지정한다.</td>
	</tr>
</table>
<hr>
<footer>
	<strong>한국경영원 인재개발원</strong>
	<address>주소입니다. 어등대로 601 길 </address>
	
</footer>