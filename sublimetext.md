### 개인용 Snippet 만들기

1. 상단 네비게이션 바 'Tools' 클릭
2. 'Developer' -> 'New Snippet' 클릭

```
<snippet>
	<content><![CDATA[
Hello, ${1:this} is a ${2:snippet}.
]]></content>
	<!-- Optional: Set a tabTrigger to define how to trigger the snippet -->
	<!-- <tabTrigger>hello</tabTrigger> -->
	<!-- Optional: Set a scope to limit where the snippet will trigger -->
	<!-- <scope>source.python</scope> -->
</snippet>
```

위 코드를 아래와 같이 수정

```
<snippet>
	<content><![CDATA[]]></content>
	<tabTrigger>hello</tabTrigger>
	<scope>source.python</scope>
</snippet>
```

content 요소 ***CDATA[]***의 '[]' 안에 커스터마이징 하고자 하는 코드 입력

```
<snippet>
	<content><![CDATA[이게 내가 자주 사용하는 코드야]]></content>
	<tabTrigger>hello</tabTrigger>
	<scope>source.python</scope>
</snippet>
```

tabTrigger 요소에 단축 이름 입력

```
<snippet>
	<content><![CDATA[이게 내가 자주 사용하는 코드야]]></content>
	<tabTrigger>myCode</tabTrigger>
	<scope>source.python</scope>
</snippet>
```

scope 요소에 text.html을 입력
*** 기본적으로는 source.sth으로 가능한데 html만큼은 앞의 source 부분을 text로 변경해줘야 함

```
<snippet>
	<content><![CDATA[이게 내가 자주 사용하는 코드야]]></content>
	<tabTrigger>myCode</tabTrigger>
	<scope>text.html</scope>
</snippet>
```

how to call snippet
snippet 사용하는 방법은, tabTrigger 요소에 입력한 trigger를 입력하고 tab 키를 누르면 자동으로 등록 코드가 작성된다.
스니펫 관련 나머지 내용

- snippet 파일들의 기본 위치
- snippet 개별 폴더 생성 및 관리
