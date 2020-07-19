---
layout: post
permalink: /mkt/gtm02_GTMInstall/
title: '웹사이트에 구글 태그 매니저(GTM) 설치하기'
date: 2020-06-14 13:30:00 +09:00
feature: '/img/posts/010/mkt_gtm02_thumbnail'
background: '/img/posts/010/mkt_gtm02_background'
categories:
  - mkt
tags:
  - 구글태그매니저
  - 구글애널리틱스
  - GA
  - GTM
  - 구글애널리틱스설치
  - 구글태그매니저설치
description: 웹사이트에 구글 태그매니저를 설치하는 방법을 소개합니다.

---

> 데이터 분석을 도와주는 구글의 서비스, **구글 애널리틱스**와 **구글 태그매니저**.

두 서비스 모두 데이터 분석을 위해 사용한다는 목적은 같지만, 동일한 서비스는 아니다. 

**구글 애널리틱스(GA)**는 조금 더 보고서에 가까운 분석 서비스를 제공하고, **구글 태그매니저(GTM)**는 그 분석을 더 잘할수 있도록 준비를 도와주는 분석 지원 서비스를 제공한다. 보고서에서 어떤 지표를 볼 것인지, 어떻게 볼 것인지 직접 설정할 수 있게 도와주는 역할을 한다.

때문에 구글 태그매니저(GTM)을 이용하면 구글 애널리틱스트(GA)를 조금 더 간편하게 설치할 수 있다. 우리가 자주 사용하는 페이스북, 네이버, 카카오도 마찬가지. 또, 매체 뿐 아니라 구글 애널리틱스 외 분석툴(앰플리튜드 등)의 스크립트도 간편하게 설치할 수 있는데, 이를 위해서는 가장 먼저 구글 태그매니저 계정을 생성하고, 구글 태그매니저의 스크립트를 웹사이트에 설치해야 한다.

------

### 구글 태그매니저 계정 생성하기

1. **구글 태그매니저(Google Tag Manager)에 접속한다.**

   [➤ 구글 태그 매니저 바로가기](https://tagmanager.google.com/)
   ![google tag manager](/img/posts/010/01.jpg)
   *태그 매니저에 로그인하면 가장 먼저 볼 수 있는 화면. 구글 태그매니저 사용을 위해서는 기본적으로 구글 계정이 필요하다.* 

2. **구글 태그매니저 내 '계정'을 생성한다.**
   ![GTM Create Account1](/img/posts/010/02.jpg)

   **계정**이란? 태그 관리자내 조직의 최상위 수준. 일반적으로 회사별로 하나만 있으면 된다. 따라서, 계정명은 보통 회사명으로 입력한다.

3. **정보 입력 후 [ 만들기 ]를 누른다.**

   ![GTM Create Account2](/img/posts/010/03.jpg)

   계정, 국가, 컨테이너, 타겟 플랫폼을 설정하고, [만들기]를 누른다. 일반적으로 계정 이름은 '회사명' 국가는 해당 비지니스를 운영하는 국가, 컨테이너 이름은 웹사이트 명을 입력한다. 타겟 플랫폼은 운영 중인 플랫폼의 형태를 선택해준다.

4. **약관 확인 후 [  예  ]를 누른다.** 

   ![GTM Create Account3](/img/posts/010/04.jpg)

   약관 확인은 필수값. 미동의시 서비스를 이용할 수 없다. (아니오 버튼을 누르면 이전 페이지로 돌아간다.)

5. **태그 관리자 설치 스크립트 [ 확인 ]을 누른다.**

   ![GTM Create Account4](/img/posts/010/05.jpg)

   태그 관리자 스크립트가 보인다면, 회원가입 완료. 아래 [ 확인 ] 버튼을 눌러준다.

------

회원가입이 완료되면 가장 먼저 컨테이너의 대시보드 역할을 해주는 **작업공간**의 **개요**를 볼 수 있다. [➤ 구성요소 설명 바로가기](https://nohze.com/mkt/gtm01_introduce/)

다음으로 태그 관리자 스니펫을 확인해 웹사이트 코드에 넣어주면, GTM 활용을 위한 기본적인 설정을 마칠 수 있다. 스니펫은 GTM-로 시작하는 7자리 컨테이너 고유번호(ID)를 누르면 언제든 확인할 수 있다.

<br>

------

### 구글 태그 매니저 스크립트 설치하기

1. **컨테이너 ID를 누른다.**

   ![GTM 컨테이너 번호](/img/posts/010/06.jpg)

   컨테이너 ID 및 스니펫은 각 컨테이너마다 고유의 값을 갖는다. 누르면, 회원가입 마지막 절차에서 봤던, 스니펫 코드를 확인할 수 있다.

2. **상단 스니펫을 복사해 웹사이트 head 영역에 넣어준다.**

   ![GTM 컨테이너 ID](/img/posts/010/07.jpg)

   ![GTM 컨테이너 ID](/img/posts/010/08.jpg)

   스니펫 코드는 안정적인 실행을 위해 가능한 위쪽에 설치해준다.

3. **하단 스니펫을 복사해 웹사이트 body 영역에 넣어준다.**

   ![GTM 컨테이너 ID](/img/posts/010/09.jpg)

   ![GTM 컨테이너 ID](/img/posts/010/10.jpg)

   body에 넣어주는 스니펫 역시 가능한 윗쪽 <body>태그 바로 뒤에 넣는다.

------

이렇게 구글 태그 매니저 스니펫만 잘 저장해두면, 이제 부터는 웹사이트 코드를 직접 조정할 일이 거의 없어진다. 특히 광고 매체의 스크립트 설치나 특정 버튼의 클릭, 스크롤 등 간단한 마케팅 이벤트는 구글 태그 매니저 내에서 충분히 설정할 수 있는데, 그 중에서도 구글 애널리틱스를 간편하게 설치 수정할 수 있다.

[➤ 구글 태그매니저로 GA 설치하기](https://nohze.com/mkt/gtm03_GAInstall/)

------

##### 📚 참고문서

- [태그 관리자 설정 및 설치하기](https://support.google.com/tagmanager/answer/6103696)
- [태그 관리자 설치전 고려사항](https://support.google.com/tagmanager/answer/6103576)
- [Google Marketing Platform 소개](https://support.google.com/tagmanager/answer/9031231)

------

실무에서 GTM을 다루며, 개인적으로 학습한 내용을 정리한 글입니다. 사실과 다른 내용이나, 문의사항이 있으시다면 댓글 또는 홈페이지 우측하단의 메신저를 보내주세요! [CONTACT](https://nohze.com/contact) 페이지를 통해 메일을 보내실 수도 있습니다. 감사합니다.<br><br>