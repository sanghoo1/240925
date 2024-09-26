# css

## navEx2

.gnb li 의 width:200; min-width:130px; 으로 주면 하위 메뉴에 리스트가 넘친다.
이것을 해결하는 방법을 배웠다.
나중에 웹사이트에서 끝에 여백이 생길때 하나하나의 요소를 눌러봐서 width
값을 조정해야한다.

선택자 ' >'  는 바로 뒤에 오는 딱 하나만 적용되는 것이 아닌 형제에도 적용된다.

	 <ul class:gnb>
		 <li>
			 <a href="#">대메뉴1</a>
		 </li>
		 <li>
			 <a href="#">대메뉴2</a>
		 </li>
 
 
 .gnb > li > a {
	 width: 100px;
	 } 
	 라고 하면 대메뉴 1만 적용되는 것이 아닌 대메뉴 2에도 적용된다.

수열선택자 nth-of-type 과 nth-of-child의 차이를 헷갈려하기에 다시 볼 필요가
있다.
헤더영역에는 보통 height 값을 부여한다는 걸 다시금 기억해야한다.
그리고 a에는 블록속성을 부여하는 게 보통이라서 li에 width값을 줘도 된다.
height 값을 a에다 주면 된다.

p>lorem  로렘생성

### aspect-ratio

반응형작업을 할때 비율에 따라 알아서 늘어난다.

youtube 긁어오기 공유-> 퍼가기 ->코드 긁기
aspect-ratio: auto; /* 기본값 */
.box2{aspect-ratio: 1 / 1;} /* 가로 기준 비율 1: 세로비율 1*/
.box7{aspect-ratio: auto  1 / 1;} /* 기본값(이미지의 경우)을 가지고 있는 경우 기본값 적용. 없는 경우 지정한 비율(1/1) 적용 */


### object-fit
.cat1{object-fit: fill;} /* 기본값. 비율 상관없이 가득 채움 */
.cat2{object-fit: contain ;} /* 비율 유지. 원본이 전부 보여짐. 대신 일부 여백이 생길 수 있음*/
.cat3{object-fit: cover; /* 비율 유지. 원본이 부모 영역을 가득 채우나 일부 가려지는 부분이 있을 수 있음*/
object-position: 50%  50%; /* 기본값 */

### 가변비디오

비디오의 width,height 값을 주고 object-fit:cover;를 주면 영역을 꽉채워준다.

### transitionBasic


/* 움직임 속성 */
transition-property: width, height, background-color; 가로,세로,백그라운드에 적용
/* 움직임 진행시간 */
transition-duration: 1s;

### transition-delay
transition 속성과 진행시간을 부여후 delay를 주면 delay의 시간 뒤에 transition이 발생한다.


# 어플리케이션 정보구조도

## 스마트문화앱 UX설계

레이블링과 내비게이션

레이블링은 짧고 사용자가 직관적으로 알 수 있게끔 이름을 지어야한다.
내비게이션은 4~5개가 이상적이다.
계층 구조도와 네비게이션 구조도는 다르다.

계층 구조도는 정보에 따른 분류이다.

네비게이션 구조도 기존에 있는 걸 확인하고 합칠건 합치고
레이블링이 개선할 게 있으면 개선한다.

네비게이션 구도조를 만들고 와이어프레임을 만든다.

내비게이션 구조도(<IA 정보구조도) 으로 퉁칠 것이다.

