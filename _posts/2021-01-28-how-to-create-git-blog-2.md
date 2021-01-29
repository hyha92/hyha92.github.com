---

title: "기술 블로그 시작하기: Github를 이용하여 블로그 만들기 (2)"  
toc: true  
toc_sticky: true  
categories:  
 - Github  
 - Git Blog  
tags:  
 - Github  
 - Git Blog  
 - minimal-mistakes  
 - Ruby  
 - Jekyll  
 - Git Clone

---

저번에 Github를 이용해서 블로그를 개설하고, Git 과 Git Desktop을 설치해보았는데요, 이번에는 블로그를 편하고 깔끔하게 관리할 수 있도록 도와주는 테마에 대해서 이야기해 볼께요!

Github 블로그는 비전문가가 하나하나 다 만들기는 조금 어려워요. 그래서 미리 잘 만들어진 테마를 가져다 쓰는게 좋아요! 오늘 저는 공개적으로 배포되어있는 테마 중 인기가 많고 제가 마음에 들었던 **minimal-mistakes** 테마를 적용시켜 볼께요.

혹시 다른 테마를 원하시는 분들은 Jekyll themes 홈페이지에서 다운받으실 수 있어요! [(Jekyll Themes 정식 홈페이지 클릭)](http://jekyllthemes.org/)

<hr/>

### A. Jekyll Theme 다운로드 (Git Clone)

우선 minimal-mistakes 테마를 다운로드 해주세요. 다음과 같이 **Code** 버튼을 눌러서 clone (복제)해주시면 되는데 두가지 방법을 알려드릴께요.

#### 1. Git Desktop 사용

저번에 받은 Git Desktop을 이용해서 바로 받아볼께요. **Open with Github Desktop**을 클릭해주세요.

![downloads](/assets/images/2021-01-28-how-to-create-git-blog-2/mmistakes_minimal-mistakes_ Jekyll theme for building a personal site, blog, project documentation, or portfolio. - Chrome 2021-01-29 오후 3_09_23.png)

Git Destop에서 다음과 같이 Repository를 clone 하려고 하는데, 첫번째는 저희가 가져오는 Repository니까 자동으로 잘 설정되어 있어요. 두번째는 저희 컴퓨터! 로컬어디에 설치하느냐 묻는건데 보시는것과 같이 local git repository에 새로운 폴더를 하나 생성하는데, 이걸 지우고 그냥 복제해주세요. 아니면 나중에 다시 옮기면 됩니다!

![downloads](/assets/images/2021-01-28-how-to-create-git-blog-2/GitHub Desktop 2021-01-29 오후 3_20_43.png)

#### b. ZIP 파일 다운로드

인터넷에서 압축 파일 많이 받으시죠? 다음과 같이 ZIP파일을 그냥 다운로드해주세요. 그러면 다운로드 폴더에 ZIP 파일이 다운로드 되어있을거에요. 다운 받고 압축을 풀어주세요.

![downloads](/assets/images/2021-01-28-how-to-create-git-blog-2/mmistakes_minimal-mistakes_ Jekyll theme for building a personal site, blog, project documentation, or portfolio. - Chrome 2021-01-29 오후 3_27_27.png)

압축을 풀면 **Downloads/minimal-mistakes-master/minimal-mistakes-master** 아래에 다음과 같이 여러 파일들이 들어있는데 전체 복사해주세요. (CTRL+A -> CTRL+C)

![downloads](/assets/images/2021-01-28-how-to-create-git-blog-2/minimal-mistakes-master 2021-01-29 오후 3_33_16.png)

그리고 블로그 만들때 생성한 Repository로 가서 붙여넣기해주세요. README 파일이 중복되면 그냥 덮어씌워주세요.

a) Git Desktop에서 Clone 하던 b) ZIP 파일 다운로드하던, 중요한건 **본인 블로그 repository에 모든 파일이 잘 복사되어있는가** 입니다.

<hr/>

### B. Quick-Start Guide 따라하기 (중요!)

다음으로는 minimal-mistakes에서 알려준 Quick-Start Guide를 따라할건데요, 이게 정말 중요해요 ㅜㅜ 저는 이걸 잘몰라서 그냥 다음 스텝 쭉 했더니 계속 에러뜨고 실패하고 난리였거든요. 꼭 따라해주세요!! (삽질은 저혼자 했던걸로...)

아래 내용은 minimal-mistakes에서 배포한 Quick-Start Guide를 따라해준거에요. 영어로 되어있어서 익숙하신분이나 자세한 설명을 알고싶으신 분은 다음을 참고해주시고, 저는 방법위주로 설명드릴께요!

참고 사이트: [Minimal Mistakes's Quick-Start Guide 공식 홈페이지 클릭](https://mmistakes.github.io/minimal-mistakes/docs/quick-start-guide/)

#### 1. Ruby 설치

Minimal Mistakes 테마 역시 Jekyll을 기반으로 만들어져있어요. 따라서 로컬에서 구동하려면 Jekyll이 필요합니다! 그리고 Jekyll은 Gem이라는 Ruby 기반 패키지가 필요해요.

Ruby 공식사이트에 들어가서 Ruby를 설치해주세요.[(Ruby 공식 홈페이지 클릭)](https://rubyinstaller.org/downloads/)

![ruby](/assets/images/2021-01-28-how-to-create-git-blog-2/Downloads - Chrome 2021-01-29 오후 3_50_18.png)

저는 최신버전중 가장 많이 사용되고있는 **Ruby+Devkit 2.7.X (x64)** 를 설치했어요 (ruby 추천!) 왼쪽에 => 표시로 굵은 글씨있는게 추천하는거니까 그거 설치해주시면되요. 설치하다 보면 **MSYS2 development toolchain** 를 설치할지 물어보는데 같이 설치해주세요.

![rubysetup](/assets/images/2021-01-28-how-to-create-git-blog-2/Setup 2021-01-29 오후 3_58_47.png)

설치를 쭉쭉 진행해줍니다. 3분? 시간걸렸어요.

![rubysetup](/assets/images/2021-01-28-how-to-create-git-blog-2/Setup 2021-01-29 오후 3_59_23.png)

완료가 되면 ridk install을 실행한다에 체크가 되어있는데 그상태 그대로 Finished 눌러주세요.

![rubysetup](/assets/images/2021-01-28-how-to-create-git-blog-2/Setup 2021-01-29 오후 4_02_48.png)

그러면 다음과 같은 창이 뜨는데 저는 1번 옵션으로 설치해주었어요. 1누르고 엔터!

![rubysetup](/assets/images/2021-01-28-how-to-create-git-blog-2/C__Windows_system32_cmd.exe 2021-01-29 오후 4_03_01.png)

엄청 열심히 뭔가를 깔다가 다음처럼 완료창이 떠요! 그럼 엔터눌러주세요. 창이 사라질꺼에요.

![rubysetup](/assets/images/2021-01-28-how-to-create-git-blog-2/C__Windows_system32_cmd.exe 2021-01-29 오후 4_07_47.png)

#### 2. Gem 설치

그 다음에는 블로그 repository에 들어가서 아래처럼 디렉토리 위치에다가 **cmd**라고 치고 엔터해주세요. 그럼 cmd가 그 repository 위치에서 열려요

![rubysetup](/assets/images/2021-01-28-how-to-create-git-blog-2/hyha92.github.io 2021-01-29 오후 4_17_35.png)

bundler을 설치해볼꺼에요. 다음과 같이 "gem install jekyll bundler"를 입력하고 엔터 눌러주세요.

```
gem install jekyll bundler
```

그리고 이제 의존성 파일들을 설치하기 위해 "bundle install"을 눌러주세요.

```
bundle install
```

#### 3. 관련 파일들 수정

그리고 파일 탐색기로 블로그 repository 위치로 가주세요. 다음과 같이 "Gemfile"이 있는데 이걸 열어주세요. 연결 프로그램은 메모장 제일 기본적으로는 메모장 선택하시면 됩니다.

![rubysetup](/assets/images/2021-01-28-how-to-create-git-blog-2/hyha92.github.io 2021-01-29 오후 4_26_19.png)

그리고 내용을 다 지우고 다음 내용을 복사 붙여넣기 해주세요. 그다음 저장해주세요. (CTRL+S)

```
source "https://rubygems.org"

gem "github-pages", group: :jekyll_plugins
gem "jekyll-include-cache", group: :jekyll_plugins
```

![rubysetup](/assets/images/2021-01-28-how-to-create-git-blog-2/Gemfile - Windows 메모장 2021-01-29 오후 4_28_39.png)

다음으로, 파일 탐색기에서 "_config.yml" 파일을 메모장으로 열어주세요.

![rubysetup](/assets/images/2021-01-28-how-to-create-git-blog-2/hyha92.github.io 2021-01-29 오후 4_29_30.png)

CTRL + F 눌러서 "Plugins" 검색해주시면, 대에충 200줄쯤에 (저는 216줄이네요) # Plugins 라고 되어있는데, 여기 "jekyll-include-cache"이 적혀있는지 확인해주세요. 없으신 분은 추가하고 저장해주세요 (CTRL+S).

```
  - jekyll-include-cache
```

![rubysetup](/assets/images/2021-01-28-how-to-create-git-blog-2/_config - Windows 메모장 2021-01-29 오후 4_35_06.png)

그다음 아까 repository 에서 열었던 cmd 창으로 돌아가서 "bundle" 이라고 치고 엔터눌러주세요.

```
bundle
```

끝나면 마지막으로 다시 파일 탐색기로 돌아가서 "_config.yml" 파일을 열어주세요. 그리고 "remote_theme"을 찾아서 (CTRL+F) 다음과 같이 수정해주세요. 못찾으시면 # Site Settings 쪽에 있어요. 저는 44 줄쯤 있었어요. 위치가 다를 수도 있어서 대충 그쯤 가서 보시면 있을것 같아요. 그리고 다른 "theme:" 이나 "remote_theme:" 부분은 다 지워주세요.

```
    remote_theme      : "mmistakes/minimal-mistakes@4.21.0"
```

![rubysetup](/assets/images/2021-01-28-how-to-create-git-blog-2/_config - Windows 메모장 2021-01-29 오후 4_39_36.png)

그리고 "url"을 찾아서 본인 블로그 주소가 잘 되어있는지 확인하시고 안되어있으면 바꿔주세요!

```
url                      : "https://UserID.github.io/"
```

![rubysetup](/assets/images/2021-01-28-how-to-create-git-blog-2/_config - Windows 메모장 2021-01-29 오후 4_54_49.png)

### C. Git Commit & Push

자 여기까지 오셨으면 로컬에서는 다 완성되었습니다! 이제는 온라인 Github 클라우드에 올려야해요. 저번에 깔아준 Github Desktop을 실행해주세요.

그리고 1~2분 후에 본인 블로그 사이트 "UserID.github.io"로 들어가서 확인해주세요! 테마가 잘 적용되면 성공!

<hr/>
