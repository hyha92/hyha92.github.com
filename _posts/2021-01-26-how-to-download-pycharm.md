---
title: "파이썬 시작하기: 파이참 설치 방법"
toc: true
toc_sticky: true
categories:
  - ColorLab
  - Python
tags:
  - Python
  - Pycharm
  - Download
  - Install
  - IDLE
  - Windows
---

파이썬을 설치완료하셨다면, 이번에는 파이참을 설치해볼께요!  

파이참은 파이썬을 개발할 수 있는 IDLE중 하나입니다.  
파이썬을 쉽고 편하게 작성할 수 있도록 해주는 IDLE은  
비주얼 스튜디오, 이클립스, 쥬피터, 파이참 등이 있습니다.  
이중에서 가장 많이 사용하는 IDLE은 쥬피터와 파이참인데요,  
쥬피터는 웹환경에서 많이 사용하고 그 이외에는 파이참을 많이 사용해요.  

그럼 파이참을 설치해 보겠습니다!

#### 1. 파이참 다운로드
파이참은 공식 홈페이지에서 최신버전으로 다운로드 가능합니다.   
<https://www.jetbrains.com/pycharm/download/#section=windows>  (링크 클릭!)  
본인의 운영체제에 맞는 파이참을 다운로드 해주세요.  
저는 파이썬과 동일하게 윈도우 64 bit 운영체제를 선택했어요.  
Professional이 Community 보다 기능이 좀더 많지만,  
저희는 무료 버전인 Community를 설치할께요!  
  
![homepage](/assets/images/2021-01-26-how-to-download-pycharm/Download PyCharm_ Python IDE for Professional Developers by JetBrains - Chrome 2021-01-25 오후 9_19_05 (1).png)
  

#### 2. 파이참 설치
다운로드된 파일을 열어주시면 다음과 같이 설치창이 보입니다.  
  
![setup](/assets/images/2021-01-26-how-to-download-pycharm/PyCharm Community Edition Setup 2021-01-25 오후 9_20_03.png)  
  
스크린샷이 조금 짤렸네요 ㅜㅜ  
Next 눌러주시면 됩니다! 
  
![setup](/assets/images/2021-01-26-how-to-download-pycharm/PyCharm Community Edition Setup 2021-01-25 오후 9_20_39.png)  
  
바로가기 원하시는분들은 Shortcut 체크해주시고, PATH 변수 업데이트에도 체크해주세요!  
저희는 파이썬 파일을 사용하기 때문에 마지막에 ".py"도 체크해주세요!  
Next 눌러주시면 됩니다.
  
![setup](/assets/images/2021-01-26-how-to-download-pycharm/PyCharm Community Edition Setup  2021-01-25 오후 9_21_41.png)  
  
시작 메뉴 폴더는 JetBrains로 되어있는데, 그대로 Next 눌러주세요.  
  
![setup](/assets/images/2021-01-26-how-to-download-pycharm/PyCharm Community Edition Setup  2021-01-25 오후 9_22_03.png)  
  
열심히 기다립니다!  

#### 3. 설치 완료
설치가 완료되면 다음과 같이 설치 완료 화면이 보입니다.   

![setup_successful](/assets/images/2021-01-26-how-to-download-pycharm/PyCharm Community Edition Setup  2021-01-25 오후 9_22_30.png)  
  
Reboot now 누르면 강제 종료되고 컴퓨터가 다시 시작됩니다.  안전하게 두번째를 선택했어요.  
2번째를 선택하면 컴퓨터를 한번 끄고 다시 시작해 주셔야 합니다!  
(PATH 설정 등 환경 설정이 필요하니 꼭 다시 시작해주세요.)    

#### 4. 파이참 설치 완료 확인
설치가 완료되었으면 시작 검색바에 Pycharm 이라고 검색해주세요.  

![setup_finished](/assets/images/2021-01-26-how-to-download-pycharm/Screenshot 2021-01-25 오후 9_29_51.png)  

설치가 잘 완료되면 보시는 것과 같이 Pycharm Community Edition이 나오는데 이걸 클릭해주세요.

![pycharm_screen](/assets/images/2021-01-26-how-to-download-pycharm/JetBrains Privacy Policy 2021-01-25 오후 9_30_06.png)  
  
개인 정보 보호 정책은 확인했다고 체크해주고, Continue 눌러주세요.  

![pycharm_screen](/assets/images/2021-01-26-how-to-download-pycharm/Welcome to PyCharm 2021-01-25 오후 9_30_33.png)  
  
다음과 같이 파이참 화면이 나오면 성공 ! (짝짝짝)

#### 5. 파이참 사용해보기

여기까지 왔으니 간단한 테스트 한번 해보고 가겠습니다!  
첫 화면에서 보이는 "New Project"를 클릭해주세요.  
  
![pycharm_test](/assets/images/2021-01-26-how-to-download-pycharm/New Project 2021-01-25 오후 9_31_51.png)  
  
프로젝트 네임은 "helloWord"라고 정해고, main.py를 생성해주도록 체크해주세요.  
그럼 다음과 같은 main 파이썬 파일이 나와요. (.py는 파이썬 파일 확장자입니다!)  
  
![pycharm_test](/assets/images/2021-01-26-how-to-download-pycharm/Screenshot 2021-01-25 오후 9_34_12.png)  

9번째줄에 빨간색 동그라미는 코드 실행시 중간에 멈춰주는 것인데, 클릭해주면 다음과 같이 사라집니다. (보통 디버깅할때 많이 사용해요.)  오른쪽 상단에 플레이모양 (삼각형)을 눌러줍니다. (실행 버튼이에요.)  
  
![pycharm_test](/assets/images/2021-01-26-how-to-download-pycharm/helloWord – main.py 2021-01-25 오후 9_34_32.png)  

하단에 실행 결과가 나오는데 저희는 Hi, {name}을 출력하도록 하였고,  
변수 {name}은 PyCharm으로 입력해주었죠! 그래서 Hi, PyCharm이라고 잘 나오네요!  
  
![pycharm_test](/assets/images/2021-01-26-how-to-download-pycharm/helloWord – main.py 2021-01-25 오후 9_34_41.png)  
  


여기까지 끝났다면 이제 파이참을 사용할 수 있어요! 
다음에는 파이썬으로 영상처리를 할 때 많이 사용하는 open CV를 알아볼께요!  :)

