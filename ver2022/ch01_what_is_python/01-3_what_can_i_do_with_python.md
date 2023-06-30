# 01-3 파이썬으로 무엇을 할 수 있을까?

## 파이썬으로 할 수 있는 일
- 시스템 유틸리티 제작
  - e.g) 고클린 등의 시스템 청소 도구 (고클린이란? )
- GUI 프로그래밍 
  - Graphical User Interface의 약자로 사용자가 편리하게 사용할 수 있도록 기능을 그래픽으로 나타낸 것
  - TK(Tkinter)라는 라이브러리를 사용하면 쉽게 GUI프로그램을 만들 수 있다.
- C/C++와의 결합
  - 속도가 중요하지 않은 부분에서는 python으로 작성하고, 속도가 중요한 곳은 C나 C++로 작성하여 결합 할 수 있다.
- 웹 프로그래밍 : `django`, `Flask`의 `Web Framework`를 사용하여 프로그래밍 할 수 있다
  - e.g) Naver, Daum 처럼 웹 사이트 제작 가능
- 수치 연산 프로그래밍 : e.g) 계산기(GUI와 어려운 수치 계산 프로그램) 
- 데이터베이스 프로그래밍 : `SQLite`, `MySQL`
- 데이터 분석 : e.g) 주가, 날씨 예측 등
  - 파이썬에서는 판다스(`pandas`)라는 좋은 라이브러리를 이용하여 쉽게 분석할 수 있다
  - 데이터 분석과 함께 많이 사용되는게 `인공지능`, `텐서플로우`를 파이썬으로 사용할 수 있다.
- 사물 인터넷 : CLOVA, NUGU, 냉장고, 세탁기, TV 등  
  - `IoT` 사물 인터넷, 각종 사물에 센서와 통신 기능을 내장하여 인터넷에 연결하는 기술

## 파이썬으로 할 수 없는 일
- 시스템과 밀접한 프로그래밍 영역 : `Windows`, `Linux`
  - 파이썬으론 운영체제를 만들지 못한다.
  - 운영체제는 C언어 또는 더 `Low Level`에 언어로 만들 수 있다.
- 모바일 프로그래밍 : 앱을 만드려면 Android : `Kotlin/Java`, ios : `Swift`
  - 앱을 만들려면 파이썬과 적합하지 않다.