---
title: SourceTree 사용법
excerpt: "유명한 쓰레기"
categories:
    - Tech
tags:
    - Git
    - SourceTree
last_modified_at: 2020-01-14T14:36:00
---

서론
===

Git은 기본적으로 터미널에서 사용하는 프로그램 입니다. 사실 모든 프로그램은 터미널에서 명령어를 실행하는 형태지만, 보급 운영체제가 도스 세대를 넘은 뒤 부턴 그래픽 인터페이스, 즉 GUI로 사용하기 편리하게 만들어진 프로그램들이 대부분입니다.

Git 또한 터미널로 사용하는 대신 GUI로 사용할 수 있도록 만들어진 여러 클라이언트가 존재합니다.

오늘은 이중에서 아마 가장 널리 알려진 소스트리에 대해 알아보도록 하겠습니다.

본론
===

## 1. 설치

1. 먼저 [소스트리 설치프로그램](https://www.sourcetreeapp.com/)을 다운로드 합니다. 
2. 다운로드된 설치 프로그램을 실행합니다.
3. 다음과 같이 Bitbucket 계정으로 로그인 합니다. 없으면 새로 가입해야 합니다.

    ![](https://chisacam.github.io/assets/image/ST_1.png)

4. 필요한 도구 설치는 체크해주고, 상세옵션은 필요에 따라 체크하면 됩니다.

    ![](https://chisacam.github.io/assets/image/ST_2.png)
    

## 2. 계정 연동

git remote 저장소로 bitbucket을 사용하는 중이 아니라면, github나 gitlab의 계정을 소스트리에 연동해주어야 정상적인 사용이 가능합니다.

이 글에서는 GitLab를 기준으로 설명하도록 하겠습니다.

도구-옵션에서 인증탭-추가를 클릭하면 다음과 같이 계정을 추가할 수 있는 팝업이 뜹니다.

![](https://chisacam.github.io/assets/image/ST_3.png)

기본 gitlab 저장소를 쓰고있다면 그냥 gitlab을 선택하면 되고, 자체 호스팅 주소를 가지고있다면 해당 주소를 기입해줍니다.

그리고 Personal Access Token 을 만들어야 하는데, gitlab의 계정 설정에서 token 메뉴로 접근하면 생성할 수 있습니다.

해당 토큰값을 입력해주면 연동이 가능합니다.

## 3. 클론

![](https://chisacam.github.io/assets/image/ST_7.png)

![](https://chisacam.github.io/assets/image/ST_8.png)

remote를 클릭해서 저장소에 있는 자료를 clone 할 수 있습니다.

## 4. 작업중인 저장소 관리

![](https://chisacam.github.io/assets/image/ST_6.png)

local이 현재 소스트리로 관리하는 git 디렉토리 목록입니다.

해당 목록중 하나를 열어서 작업하거나, 새 폴더를 만들고 git 디렉토리로 설정할 수 있습니다.

## 5. 실행중 모습

![](https://chisacam.github.io/assets/image/ST_5.png)

왼쪽에는 브랜치와 저장소 목록이, 중앙에는 커밋로그와 브랜치 그래픽, 그리고 하단에는 커밋로그의 상세정보가 표시됩니다.

상단에 있는 커밋, pull, push, 패치, 브랜치 등의 메뉴가 각각 Git의 메뉴들과 동일하게 동작합니다. 원하는 브랜치를 선택하고 그저 버튼만 클릭하면 됩니다. (아쉽게도 커밋로그까지 소스트리가 써주진 않습니다 ^^)

결론
===

터미널에서 명령어를 입력해서 처리했던 내용들을 GUI툴을 이용하면 클릭으로 할 수 있게됩니다. 사용에 익숙해진다면 작업 속도도 더 빨라지고, 터미널로도 볼 수 있긴 하지만 더 좋은 그래픽과 가독성을 가진 전체 브랜치, 커밋 상황을 볼 수도 있었습니다.

하지만 소스트리 프로그램 자체가 좀 불안정하고, 설치시 무조건 bitbucket 계정이 필요한점, 그리고 설정이 소소하게 불편한점은 단점입니다.(옵션으로 OpenSSH선택이 가능하긴 하지만 기본 ssh 클라이언트도 putty를 사용...)

따라서 다음에는 더 나은 클라이언트를 소개하도록 하겠습니다.

참고자료
===

https://www.sourcetreeapp.com/