---

title: "기술 블로그 시작하기: Github를 이용하여 블로그 만들기 (1)"  
toc: true  
toc_sticky: true  
categories:  
 - Github  
 - Git Blog  
tags:  
 - Github  
 - Git Blog

---

제가 Github로 블로그를 만들겠다고 생각하고, 시행착오를 겪었는데 오늘 정리해서 올려볼께요! 초보자 분들도 만들 수 있도록 최대한 자세히 설명드리려고 해요.

<hr/>

### A. Github 계정 및 Repository 생성

#### 1. Github 계정 만들기

Github로 블로그를 만들려면, 우선 Github 계정이 필요합니다. 계정이 있다면 다음단계로 가고, 계정이 없다면 만들어 봅시다! 우선 Github 홈페이지에 들어가주세요. [(Github 공식 홈페이지)](https://github.com/)

오른쪽 상단에 회원 가입 (Sign up)을 눌러주세요. 차례대로 아이디, 비밀번호, 홍보성 광고 메일 구독 체크 유무, 사람 인증을 끝내고 계정을 생성해주세요.

#### 2. 블로그용 Repository 생성

그다음은 보시는것과 같이 Repository 이름을 생성할건데 **Repository name을 반드시 "UserID.github.io" 로 설정해주세요.** 예를들어 저는 아이디가 hyha92라서 hyha92.github.io로 설정해주었어요. 블로그를 할거니까 Public (공개)을 설정해주시고, 저는 README 파일 자동생성을 체크해주었어요.

![Repository](/assets/images/2021-01-28-how-to-create-git-blog-1/Create a New Repository - Chrome 2021-01-28 오후 9_35_20.png)

#### 3. 블로그 사이트 확인

잘 생성이 되었다면, UserID.github.io로 접속이 가능합니다. 그리고 본인의 Repository에 오시면 다음 그림처럼 setting 버튼이 있어요.

![setting](/assets/images/2021-01-28-how-to-create-git-blog-1/hyha92_hyha92.github.io - Chrome 2021-01-28 오후 9_45_15.jpg)

setting 버튼을 누르면 설정 메뉴가 뜨는데, Options -> Settings 에 보시면 Repository name 이 UserID.github.io로 잘 생성되었는지 확인해주세요.

![check](/assets/images/2021-01-28-how-to-create-git-blog-1/Options - Chrome 2021-01-28 오후 9_51_53.jpg)

여기까지 잘 생성되었으면 주소창에 UserID.github.io를 치고 블로그 사이트가 잘 생성되었는지 확인할 수 있어요! 아직 아무것도 없는 깡통 사이트지만 이제부터 예쁘게 바꿔볼께요!

<hr/>

### B. Git & Github Desktop 설치하기

#### 1. Git 이란 무엇인가

다음으로는 가장 근본이 되는 Git과 Github가 무엇인지 간단하게 설명드릴께요. 제일 쉬운 설명은 **코드를 공동작업하기위한 서비스**라고 저는 생각해요. 쉽게 말해서 코드를 여러사람이 코드를 같이 작업하는데 ver1, ver2, ver3처럼 여러 버전이 오가고 누구는 중간에 수정하고 그래서 꼬이고 그러잖아요? 그런걸 똑똑하게 관리해주는 시스템이에요. Onedrive나 Dropbox 같은 시스템인데 코드용이라고 생각하면 편해요! 여기서 Git은 로컬에서 버전을 관리하는 운영 방식이고, Github는 온라인 클라우드 서버를 이용해서 버전을 관리해주는 거에요. 따라서 내 컴퓨터에서는 Git으로 로컬 저장소에 저장하고, 이를 공유하기위해 Github에 업로드한다고 생각하면 됩니다! 반대로 다른사람들이 올린 코드를 받고싶으면 Github에서 Git으로 내 컴퓨터(로컬)로 가져오면 되는거죠.

핵심은 본인이 커밋(결제 요청 같은 것)하고 Push(업로드)하면 아까 저희가 이름지은 저장소에 저장이되고 드랍박스처럼 오프라인 데스크탑과 온라인 저장소가 연동이 가능해요. 이때 오프라인 데스크탑에서 온라인 저장소로 파일을 올리는게 "Push", 온라인 저장소에서 오프라인 데스크탑으로 파일을 동기화시키는게 "Pull"이에요.

> **"Push"**: Offline Desktop (Local) -> Online Repository  
> **"Pull"**: Online Repository -> Offline Desktop (Local)

내가 폴더창에서 파일을 직접 열고 수정했다면 커밋 후 Push를, 온라인 github에서 글을 작성했다면 동기화를 위해 로컬 데스트탑에 Pull을 해주면 됩니다. 온라인 오프라인 마음대로 저장하면 충돌해서 커밋할 수 없어요. 추후 다시 설명드릴께요!

#### 2. Git 설치하기

Git은 공식 홈페이지에서 본인 컴퓨터 사양에 맞는 것으로 설치해주세요. [(Git 공식 홈페이지 클릭)](https://git-scm.com/downloads)

설치는 별다른 것 없이 Next만 눌러주시고 완료해주시면 됩니다! 완료가 되면 시작메뉴에서 "cmd"를 실행시키고, 다음과 같이 "git --version"을 입력후 버전이 뜨면 잘 설치된 것입니다.

```
$ git --version
```

![gitVersion](/assets/images/2021-01-28-how-to-create-git-blog-1/선택 명령 프롬프트 2021-01-28 오후 10_34_09.png)

#### 3. Github Desktop 설치하기

다음으로는 Github Desktop을 설치해볼께요. 사실 그냥 온라인으로 해도되고, 매번 cmd를 이용해서 명령어를 사용해도 되지만, 써보니까 UI도 좋고 훨씬 직관적이고 편하더라구요! 특히 아직 프로그래밍이 익숙하지 않으신분들은 개념만 알면 쉽게 사용가능합니다! **(Commit -> Push / Pull)**

Github Desktop을 공식 사이트에 가서 설치해주세요. [(Github Desktop 공식 홈페이지 클릭)](https://desktop.github.com/)

설치는 크게 어려운것 없이 로그인해 설치 완료하시면 됩니다. 제가 스크린샷이 없네요 ㅜㅜ

로그인하시고 오른쪽에보면 **Your repositories** 아래에 UserID/UserID.github.go 라는 Repository가 있을거에요. 클릭해서 연동해주시면 됩니다!

<hr/>

여기까지 끝났다면 기본적인 설치는 다 끝났고, 다음에는 블로그의 꽃! 테마 적용 방법을 알아보도록 할께요! 감사합니다 : )
