# DeliveryProject(배달서비스 프로젝트)

# 프로젝트 기획안
### 작성일 : 2022. 01. 27
### 작성자 : 박선영
# 프로젝트 명 : 배달시켜 
## 1. 기획 의도 
### 목적
- 배달의 민족, 요기요와 같은 배달어플 서비스를 웹상으로 구현해보고자 했다. 소비자에게 는 주문, 결제, 실시간 배달현황, 환불, 리뷰 등의 서비스를, 점주에게는 주문관리, CRM시스템 등의 서비스를 제공한다. 
### 프로젝트 기획배경
- 코로나19 이후 집에 거주하는 인구가 많아지면서 소비자들의 음식배달 어플 사용률이 확연히 늘어났다. 이같은 현상은 앞으로도 지속될 것으로 보이며, 사용자들이 더욱 더 편리한 서비스를 이용할 수 있는 배달시스템의 필요성을 느꼈다. 
### 어떤 것들이 가능한가
- 기존 배달 어플리케이션을 벤치마킹해 각각의 배달앱에서 제공하고 있는 서비스와 기능들을 구현해보고자 한다. 
## 벤치마킹 
### 배달의민족, B마트
	 1. 특징
	바쁜 현대인들에게 시간은 금인데 식당이나 마트에 직접 찾아갈 필요 없이 손가락 하나만으로 손쉽게 먹고싶은 음식이나 필요한 물품들을 바로 주문할 수 있다. 점주 페이지에서 주문관리를 할 수 있다 

## 주요 기능 (고객 / 점주)
### 4-1. 공통
### A. 회원가입
	- 고객/점주를 구분해서 회원가입
	- 회원가입 시 이메일 중복확인, 비밀번호 유효성 검사, 공백일 시 에러메시지<br>
### B. 로그인
	- 아이디, 비밀번호 일치여부 확인 후 로그인
	- 로그인 후 로그인하기 전 있던 페이지로 이동<br>
### C. 리뷰작성 
- 로그인한 아이디를 작성자로 사용
- 고객이 주문 후 리뷰를 작성할 수 있으며, 점주는 대댓글 작성 가능 
- 별점평가(1~5), 추천/비추천<br>
### 4-1. 고객
### A. 주문하기
	- 메뉴선택(radio), 수량변경, 선택했던 메뉴 삭제 
	- 배달방법 선택 : 배달 / 포장
### B. 장바구니
	- 장바구니에서 한꺼번에 결제 가능
### C. 결제 
	- 카드/현금결제 
	- 배달원/점주에게 요청사항 기입란 有 
	- 현금영수증 
	- 등록된 쿠폰이 있으면 할인 가능('내 쿠폰' 버튼 누르고 들어가서 사용가능)
### D. 환불
### E. 배달 예상시간 및 실시간 배달추적기능
	- 소켓 이용 
	- api 활용하기 : 구글맵 또는 인터랙티브 지도  
	- 주문상태 : 푸쉬알림
### F. 주문취소, 다시 주문하기
	- 주문취소내역에서 다시 주문 가능하도록(?) 
### G. 프로모션 코드 & 쿠폰관리
	- 코드 입력해서 쿠폰등록 
	- 내 쿠폰함에서 쿠폰관리 
### 4-2. 점주
### A. 주문관리 : 주문 접수/취소 등의 action을 취했을 시 고객에게 알림이 뜨도록
- 왼쪽 메뉴바 : 처리중, 완료, 매출조회, 일정관리 
- 영업중 / 영업중지 선택, 배달
- 주문목록 : 날짜별 조회 가능 
- 주문 상세조회(주문전표) 
    1) 요청사항(가게/배달원), 주문내역, 배달주소, 고객연락처, 주문번호, 주문시간, 가게정보확인
    2) 상단에 예상시간 기입 후 확인버튼을 누르면 주문 접수 
  - 주문 접수 시 주문한 고객에게 '접수완료' 알림뜨도록 
  - 주문 취소 : 들어온 주문을 취소할 수 있음  

## 5. 기타 
 - 고객 / 점주 페이지를 따로 구분(로그인 역시 그 페이지에서 가능하도록) 


