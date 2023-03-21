﻿# 네이버 지도에서 가게 정보 스크랩핑하기
프로그라피 '케이크크' 서비스를 만들며 많은 케이크샵의 정보가 필요했는데,,
<br>
자동화를 하면 훨씬 간편할 것이라고 생각했다. (이래서 개발을 하나보다.. 너무 좋더라,,)
<br>
그래서 나 대신 가게 데이터 쌓아줄 <strong>첫 Scraping!</strong>


### 실행 화면


https://user-images.githubusercontent.com/81179951/226692192-450bb4d4-3b0a-44ec-8f6f-5b6a3acbd38f.mp4

케이크샵의 이름, 주소, 공유 URL을 찾아 csv에 데이터를 넣어준다.
<br>
csv에 들어가는 데이터: <strong>담당자, 가게 이름, 구 위치, 주소, 케이크 종류(는 긁어올 수 없는 데이터라 빈칸으로), 링크 </strong>
![image](https://user-images.githubusercontent.com/81179951/226693271-fd0c6951-d751-4ca6-9b21-370c725a2177.png)


### 사용 방법
1. 크롬 버전과 내 os에 맞는 chromedriver를 설치
https://chromedriver.chromium.org/downloads
2. 프로젝트 속에 chromedriver를 넣고 scraping.py에서 driver의 위치 지정해주기
3. selenium package 설치
4. 담당자 이름 'NAME'과 지역 이름 'LOCATION' 설정하기
5. 실행


<br>

#### 그 외) 크롤링과 스크랩핑 차이
웹 크롤링은 웹 페이지들의 링크를 통해 계속해서 정보를 찾아 나아감.
<br>
웹 스크래핑은 특정 웹 사이트에서만 데이터를 추적함.
