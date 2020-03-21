---
title: Github blog 만들기
description: 정적사이트인 jekyll을 활용한 Github blog 제작 과정을 소개합니다.
categories:
 - Github
tags: Github, jekyll, Git, NexT Theme
---

>{: .[window 환경]-center}
다양한 블로그 중에서 직접 꾸밀 수 있고 나만의 특별한 블로그를 제작하고 싶어 검색하다 Github를 알게 되어 시작하게 되었습니다.



<!-- more -->

[Github](https://github.com/) Github 사이트
[jekyll](https://jekyllrb-ko.github.io/) 한글 번역 사이트
[git](https://git-scm.com/) Git 사이트


## 1. github 가입

* [Github](https://github.com/)
사이트에 접속해 버전에 맞는 가입을 합니다.
![Desktop Preview](C:\ds-go.github.io\photo\github.jpg)

## 2. git 설치

* [git](https://git-scm.com/) 사이트에 접속해 버전에 맞는 git을 설치합니다.
![Desktop Preview](C:\ds-go.github.io\photo\git.jpg)

## 3. git 사용자 등록

* **Git Bash**를 실행하고 다음을 한줄 씩 입력합니다.
```sh
git config --global user.name "깃허브네임"
git config --global user.email "깃허브이메일"
```
![Desktop Preview](C:\ds-go.github.io\photo\git_01.jpg)


## 4. github 로그인 및 jekyll theme 계정에 Fork

* google에서 '지킬 테마'를 검색 또는 [jekyll Themes](http://jekyllthemes.org/)에 접속하여 Next Theme 또는 원하는 Theme를 클릭하고, Homepage에 접속해 우측 상단 Fokr를 눌러 자신의 계정에 복제합니다.

![Desktop Preview](C:\ds-go.github.io\photo\jekylltheme.jpg)
![Desktop Preview](C:\ds-go.github.io\photo\next_homepage.jpg)


## 5. Repositories rename
잠시 기다리면 Fork 완료한 상태가 나타나게 되는데 이때 Setting에서 Repository name을 **'깃허브네임.github,io'**로 변경한 후 Rename을 클릭합니다. 향후 위 name이 자신의 주소가 됩니다.
**깃허브네임과 일치하지 않으면 나중에 로컬과 연동할 때 에러가 발생하게 돼요.**
![Desktop Preview](C:\ds-go.github.io\photo\repositories_rename.jpg)

Setting에서 스크롤을 아래로 내리다 보면 Github Pages 아래부분이 초록색으로 나올 경우 개설이 완료됐다는걸 뜻한답니다.
![Desktop Preview](C:\ds-go.github.io\photo\githubpages.jpg)
주소로 접속하면 적용한 THeme와 함께 페이지가 나타나는데요. 사용자들 마다 다르게 5분안으로 페이지가 적용되어 나타난다고 합니다.
![Desktop Preview](C:\ds-go.github.io\photo\dsgogithub.jpg)


!@#!%@#!$




## 2.git 설치

* [git](https://git-scm.com/)
사이트에 접속해 버전에 맞는 git을 설치합니다.
![Desktop Preview](C:\ds-go.github.io\photo\git.jpg)

## 2.git 설치

* [git](https://git-scm.com/)
사이트에 접속해 버전에 맞는 git을 설치합니다.
![Desktop Preview](C:\ds-go.github.io\photo\git.jpg)


* Sidebar

![Desktop Sidebar Preview](http://iissnan.com/nexus/next/desktop-sidebar-preview.png)

* Sidebar (Post details page)

![Desktop Sidebar Preview](http://iissnan.com/nexus/next/desktop-sidebar-toc.png)

* Mobile

![Mobile Preview](http://iissnan.com/nexus/next/mobile.png)


## Installation

Check whether you have `Ruby 2.1.0` or higher installed:

```sh
ruby --version
```

Install `Bundler`:

```sh
gem install bundler
```

Clone Jacman theme:

```sh
git clone https://github.com/Simpleyyt/jekyll-theme-next.git
cd jekyll-theme-next
```

Install Jekyll and other dependencies from the GitHub Pages gem:

```sh
bundle install
```

Run your Jekyll site locally:

```sh
bundle exec jekyll server
```

More Details：[Setting up your GitHub Pages site locally with Jekyll](https://help.github.com/articles/setting-up-your-github-pages-site-locally-with-jekyll/)


## Features

### Multiple languages support, including: English / Russian / French / German / Simplified Chinese / Traditional Chinese.

Default language is English.

```yml
language: en
# language: zh-Hans
# language: fr-FR
# language: zh-hk
# language: zh-tw
# language: ru
# language: de
```

Set `language` field as following in site `_config.yml` to change to Chinese.

```yml
language: zh-Hans
```

### Comment support.

NexT has native support for `DuoShuo` and `Disqus` comment systems.

Add the following snippets to your `_config.yml`:

```yml
duoshuo:
  enable: true
  shortname: your-duoshuo-shortname
```

OR

```yml
disqus_shortname: your-disqus-shortname
```

### Social Media

NexT can automatically add links to your Social Media accounts:

```yml
social:
  GitHub: your-github-url
  Twitter: your-twitter-url
  Weibo: your-weibo-url
  DouBan: your-douban-url
  ZhiHu: your-zhihu-url
```

### Feed link.

> Show a feed link.

Set `rss` field in theme's `_config.yml`, as the following value:

1. `rss: false` will totally disable feed link.
2. `rss:  ` use sites' feed link. This is the default option.

    Follow the installation instruction in the plugin's README. After the configuration is done for this plugin, the feed link is ready too.

3. `rss: http://your-feed-url` set specific feed link.

### Up to 5 code highlight themes built-in.

NexT uses [Tomorrow Theme](https://github.com/chriskempson/tomorrow-theme) with 5 themes for you to choose from.
Next use `normal` by default. Have a preview about `normal` and `night`:

![Tomorrow Normal Preview](http://iissnan.com/nexus/next/tomorrow-normal.png)
![Tomorrow Night Preview](http://iissnan.com/nexus/next/tomorrow-night.png)

Head over to [Tomorrow Theme](https://github.com/chriskempson/tomorrow-theme) for more details.

## Configuration

NexT comes with few configurations.

```yml

# Menu configuration.
menu:
  home: /
  archives: /archives

# Favicon
favicon: /favicon.ico

# Avatar (put the image into next/source/images/)
# can be any image format supported by web browsers (JPEG,PNG,GIF,SVG,..)
avatar: /default_avatar.png

# Code highlight theme
# available: normal | night | night eighties | night blue | night bright
highlight_theme: normal

# Fancybox for image gallery
fancybox: true

# Specify the date when the site was setup
since: 2013

```

## Browser support

![Browser support](http://iissnan.com/nexus/next/browser-support.png)
