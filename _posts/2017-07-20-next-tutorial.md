---
title: Github blog 만들기
description: 정적사이트인 jekyll을 활용한 Github blog 제작 과정을 소개합니다.
categories:
 - Github
tags: Github, jekyll, Git, NexT Theme

```sh
[window 환경]
```
---

>안녕하세요. Github Blog를 처음으로 시작하게되어 제작 과정을 소개하고자 합니다. 다양한 블로그 중에서 직접 꾸밀 수 있고 나만의 특별한 블로그를 제작하고 싶어 GIthub를 시작하게 되었습니다. 초보자인 저를 포함한 처음 접하는 분들을 위한 설명으로 다소 부족한 점이 있어 참고용 정도로만 보시면 좋을거 같아요!



<!-- more -->


## github 가입

* [Github](https://github.com/)
사이트에 접속해 버전에 맞는 가입을 합니다.
![Browser support](https://raw.githubusercontent.com/DS-GO/ds-go.github.io/master/photo/github.jpg)

## git 설치

* [git](https://git-scm.com/) 사이트에 접속해 버전에 맞는 git을 설치합니다.
![Browser support](https://raw.githubusercontent.com/DS-GO/ds-go.github.io/master/photo/git.jpg)

## git 사용자 등록

* **Git Bash**를 실행하고 다음을 한줄 씩 입력합니다.
```sh
git config --global user.name "깃허브네임"
git config --global user.email "깃허브이메일"
```
![Browser support](https://raw.githubusercontent.com/DS-GO/ds-go.github.io/master/photo/git_01.jpg)


## github 로그인 및 jekyll theme 계정에 Fork

* google에서 '지킬 테마'를 검색 또는 [jekyll Themes](http://jekyllthemes.org/)에 접속하여 Next Theme 또는 원하는 Theme를 클릭하고, Homepage에 접속해 우측 상단 Fokr를 눌러 자신의 계정에 복제합니다.

![Browser support](https://raw.githubusercontent.com/DS-GO/ds-go.github.io/master/photo/jekylltheme.jpg)
![Browser support](https://raw.githubusercontent.com/DS-GO/ds-go.github.io/master/photo/next_homepage.jpg)


## Repositories rename
잠시 기다리면 Fork 완료한 상태가 나타나게 되는데 이때 Setting에서 Repository name을 **'깃허브네임.github,io'**로 변경한 후 Rename을 클릭해 줍니다. 향후 위 name이 자신의 주소가 된다고 하네요.
**깃허브네임과 일치하지 않으면 나중에 로컬과 연동할 때 에러가 발생하게 돼요.**
![Browser support](https://raw.githubusercontent.com/DS-GO/ds-go.github.io/master/photo/repositories_rename.jpg)

Setting에서 스크롤을 아래로 내리다 보면 Github Pages 아래부분이 초록색으로 나올 경우 개설이 완료됐다는걸 뜻한답니다.
![Browser support](https://raw.githubusercontent.com/DS-GO/ds-go.github.io/master/photo/githubpages.jpg)
주소로 접속하면 적용한 THeme와 함께 페이지가 나타나는데요. 사용자들 마다 다르게 5분안으로 페이지가 적용되어 나타난다고 합니다.
![Browser support](https://raw.githubusercontent.com/DS-GO/ds-go.github.io/master/photo/dsgogithub.jpg)






## Blog에 게시글 등록

* [haroopad](http://pad.haroopress.com/)
Githu blog는 MarkDown 형식이기 때문에 게시글을 등록하기에 앞서 MarkDown 프로그램을 사용해야 하는데요. 저는 무료 한글버전인 haroopad를 사용해 작성했습니다. Haroopad를 사용하시고자 하는 분은 위 사이트에서 User를 클릭하시면 각 운영체제에 맞는 버전을 다운받으 실 수 있습니다.
![Browser support](https://raw.githubusercontent.com/DS-GO/ds-go.github.io/master/photo/haroopad.jpg)

## Github 원격저장소와 로컬 저장소 연동하기

Github에 저장되어 있는 NexT Theme 자료를 로컬영역 C드라이브로 불러와서 수정하기 위해 다음과 같은 명령어를 입력합니다.
**[Git Bash를 컴퓨터를 종료하였거나 처음 실행한다면 Git 사용자 등록을 다시 한번 해주시면 됩니다.]**

```sh
cd c:/
git clone https://github.com/깃허브닉네임/레퍼지토리이름
```

![Browser support](https://raw.githubusercontent.com/DS-GO/ds-go.github.io/master/photo/gitclone.jpg)
저는 이미 만들어 놓은 상태여서 위와 같은 문구가 나오는데요. 제대로 작성 하셨다면 
```sh
Cloning into.............
remote: ......
remote: ......
Receiving deltas: 100% ~~.....
```
라는 문구가 나타나게 되며 지정한 경로에 폴더가 생성됩니다.
![Browser support](https://raw.githubusercontent.com/DS-GO/ds-go.github.io/master/photo/localclone.jpg)


## Blog 게시물 작성하기
Github에서 불러온 파일의 목록을 살펴보면 여러가지가 들어있습니다. 그 중에서 **_posts** 파일이 우리가 게시물을 작성하게 될 데이터를 보관하는 파일입니다. 각 Theme 마다 파일명이 다를 수 있으므로 자세한 정보를 원하면 다운로드를 받은 Theme 홈페이지에 접속하면 확인 할 수 있습니다.

수정하고자 하는 md파일을 불러온 후, MarkDown 양식에 맞춰 글을 작성하고 저장하면 끝입니다. 그렇다고 홈페이지에 바로 적용되는 것이 아니라 파일을 다시 Github에 업로드를 완료해야 게시글이 수정되므로 업로드 하는 과정을 진행합니다.
![Browser support](https://raw.githubusercontent.com/DS-GO/ds-go.github.io/master/photo/haroo_bloging.jpg)


## 작성한 글 Github에 Upload 하기
Git Bash 창에 아래 명령어를 순서대로 입력합니다.
```sh
> cd 깃허브닉네임.github.io
	-> Github 저장소 이동 명령어
> git status
	-> 파일 상태 확인, 수정 및 삭제된 파일일 경우 하단에 붉은색 글자로 표시
> git add *
	-> 새로 만들어진 파일을 Upload
> git status
	-> 새로 만들어진 파일이 존재하면 초록색 글자로 표시
```
![Browser support](https://raw.githubusercontent.com/DS-GO/ds-go.github.io/master/photo/githubupload.jpg)


## Upload 한 파일 commit 하기
Upload한 파일을 최종적으로 Github에 올리기 위해 작업을 확정하고 저장소에 반영하는 작업을 실행합니다.
```sh
> git commit -m "커밋메시지"
	-> 커밋메시지 경우 활동 기록을 위해 작성
> git status

> git remote -v
	-> Uploda한 파일이 내 Github 저장소가 맞는지 확인
> git push
	-> 최종 완료 작업
```
![Browser support](https://raw.githubusercontent.com/DS-GO/ds-go.github.io/master/photo/githubpush.jpg)


이제 홈페이지에 접속해서 확인해보시면 됩니다.
![Browser support](https://raw.githubusercontent.com/DS-GO/ds-go.github.io/master/photo/complete.jpg)








