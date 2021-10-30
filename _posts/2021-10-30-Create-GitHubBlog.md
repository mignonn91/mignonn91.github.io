---
title: '프로그래밍: GitHub 블로그 제작하기'
categories:
- Action
tags:
- 프로그래밍
toc: true
toc_sticky: true
toc_label: 목차
---

본 과정은 Window10 환경에서 진행된다.

## Step 1. Git 설치
이미 설치한 관계로 넘어간다.

## Step 2. repository 만들기
깃허브 페이지가 들어갈 저장소 제작을 한다.
Github에 접속해서, 계정 메뉴에서 new Repository를 선택한다. 그리고, 저장소를 {사용자이름}.github.io 형식으로 만든다.

**{사용자이름}으로 하지 않을 경우 오류가 발생할 수 있다.**


## Step 3. 블로그 테마 찾기
[http://jekyllthemes.org/]({{"http://jekyllthemes.org/"}}){:target="_blank"}<br>
[https://jekyllthemes.io/free]({{"https://jekyllthemes.io/free"}}){:target="_blank"}<br>
[https://jamstackthemes.dev/ssg/jekyll/]({{"https://jamstackthemes.dev/ssg/jekyll/"}}){:target="_blank"}<br>
[https://jekyll-themes.com/free/]({{"https://jekyll-themes.com/free/"}}){:target="_blank"}<br>
[http://themes.jekyllrc.org/]({{"http://jekyllthemes.org/"}}){:target="_blank"}<br>
[https://jekyllthemes.io/]({{"https://jekyllthemes.io/"}}){:target="_blank"}<br>

주소들을 참고하여 'minimal-mistakes' 테마를 선택하고  Fork를 이용하여 저장소로 불러온다.

## Step 4. Jekyll 설치
[http://jekyllrb-ko.github.io/]({{"http://jekyllrb-ko.github.io/"}}){:target="_blank"} 에 접속하여 Jekyll을 설치하고 다음 명령어들을 실행한다.<br>

```java
# gem install bundler
# bundle
# jekyll serve
```

만약 오류가 뜬다면,

```java
# bundle install
# bundle add webrick
# bundle exec jekyll serve --trace
```

위 내용으로 해결 가능하다.

## Step 5. 로컬서버 접속
[http://127.0.0.1:4000]({{"http://127.0.0.1:4000"}}){:target="_blank"} 위 주소로 접속하면 로컬서버 접속이 가능하다.

## Step 6. 실제 사용을 위한 작업
[https://honbabzone.com/jekyll/start-gitHubBlog/#_configyml-%EC%88%98%EC%A0%95]({{"https://honbabzone.com/jekyll/start-gitHubBlog/#_configyml-%EC%88%98%EC%A0%95"}}){:target="_blank"} 
### _config.yml 파일 수정
위 주소를 참고하여 자신의 용도에 맞게 _config.yml 파일을 수정한다.

### navigation 설정
위 주소를 참고하여 카테고리를 만든다.

## Step 7. Admin 세팅
Post 작성 시 좀 더 직관적인 화면으로 하고 싶을 때 수행한다.

### Gemfile 수정
```java
gem 'jekyll-admin', group: :jekyll_plugins
```
### 명령어 수행
```java
# bundle install
# jekyll serve 
```
## 참고사이트
[공개, 비공개] <https://codedragon.tistory.com/8740> <br>
[git clone 명령어]<https://www.lainyzine.com/ko/article/git-clone-command/> <br>
[비공개 git clone] <https://mparchive.tistory.com/153> <br>
[git blog 만들기] <https://zeddios.tistory.com/1222> <br>
[github 블로그 시작하기] <https://oilmlio.com/blog/How-to-Create-a-GitHub-Blog/> <br>
[github 레파지토리 삭제] <https://coding-factory.tistory.com/246> <br>
[github 블로그 만들기] <https://velog.io/@zawook/Github-%EB%B8%94%EB%A1%9C%EA%B7%B8-%EB%A7%8C%EB%93%A4%EA%B8%B0-1> <br>
[Windows 환경에서 github 블로그 제작] <https://iingang.github.io/posts/windows-github-set/#%EB%A1%9C%EC%BB%AC-repository-%EC%83%9D%EC%84%B1-%EB%82%B4-%EA%B9%83%ED%97%88%EB%B8%8C%EC%99%80-%EC%97%B0%EB%8F%99> <br>
[--trace 오류] <https://velog.io/@minji-o-j/jekyll-%EC%98%A4%EB%A5%98-%ED%95%B4%EA%B2%B0><br>
[--webrick 오류해결] <https://github.com/jekyll/jekyll/issues/8523> <br>
[git Blog 만들기] <https://honbabzone.com/jekyll/start-gitHubBlog/#step-3-%EB%A1%9C%EC%BB%AC-%EA%B0%9C%EB%B0%9C-%ED%99%98%EA%B2%BD%EC%9D%84-%EC%9C%84%ED%95%9C-%EB%A3%A8%EB%B9%84%EC%84%A4%EC%B9%98> <br>[Git 에러 CRLF will be replaced by LF] https://blog.jaeyoon.io/2018/01/git-crlf.html

## Comment
Tistory와 NaverBlog에서 느꼈던 **부족함**을 해결하기 위해 본 과정을 진행하였다.<br>Github Blog를 제작하기 위해서는 **HTML**, **CSS**, **Node.js** 그리고 **Markdown 문서**에 대한 공부가 매우 필요하다. <br>현재로서는 폭 넓은 사용이 **불가능**하다.<br>Github Blog의 사용을 **보류**한다.<br>왜 안올라가는 걸까요?
