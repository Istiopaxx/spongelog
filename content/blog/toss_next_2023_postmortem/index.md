---
title: 'Toss(토스) NEXT 2023 공채 후기'
date: 2023-08-05
tags: [Postmortem, Job]
description: 토스 NEXT 2023 공채 후기입니다.
---

# 토스 NEXT 2023

취준을 시작하며, 가고 싶은 회사들이 있었다. 토스도 그 중 하나였다.
근데 내가 가고 싶은 회사들은 기술 스택으로 `Node + Nestjs`를 사용하는 회사가 얼마 없었다.
이쯤 되면 가고 싶은 회사를 늘리던지, 기술 스택을 늘리던지, 기술이 안맞아도 지원해야 하는게 아닐까?
하는 생각 중에 토스 NEXT 공채를 보게 되었고, 내 상황을 판단할 좋은 기회라고 생각하여 지원하였다.
`Node.js(Web Automation)` 직군으로 지원하였고, 최종 결과는 **문화 적합성 면접 탈락**.
전 과정을 돌아보며 무엇을 잘했고 못했는지 돌이켜보자.

### 토스 Node.js(Web Automation) 직군

보통 `Node.js`(이하 노드)는 백엔드 서버 쪽의 기술 스택으로 쓰는게 일반적이라고 생각해왔다.
하지만 토스의 `Node.js` 직군은 `Web Automation` 기술에 노드를 사용한다.
나는 `WA` 기술을 간단히 말하자면 웹 브라우저 환경에서만 할 수 있는 일들을 자동화하는 기술이라고 이해했다.
예를 들어 나는 핀테크 서비스인 **토옷** 개발자이고, **토옷** 서비스에서는 사용자의 여러 은행 계좌의 입출금 내역을 가져와야 하는 작업이 필요하다고 하자.
은행 웹사이트의 서버가 보안상의 이유로 계좌 입출금 내역을 확인할 수 있는 `API`가 열려있지 않다고 한다면, 토옷 서비스는 계좌 입출금 내역을 가져오기 위해 마치 사용자인 것처럼 행세하며 은행 웹사이트에 접속해 사용자인 것처럼 아이디/비번/기타 필요한 인증을 수행하고 계좌 입출금 내역을 확인해야 한다.
이 때 사용되는 기술이 `WA` 기술이고, 브라우저와 서버를 왔다갔다 하며 데이터를 스크래핑해야 하기 때문에 브라우저/서버 모두에서 쓰이는 언어인 `js` 및 노드를 활용한다고 볼 수 있다.

## 코딩 테스트

코딩 테스트의 문제들은 `javascript`로만 풀 수 있었고, 프로그래머스에서 진행되었다.
서버나 코어 뱅킹 직군에서는 코딩 문제 + 서술형 문제로 나온다고 보았으나 노드 직군은 코딩 문제 7문제로 출제되었다.
전체적으로 어려운 알고리즘을 써야 하거나 해결 방법 자체를 생각해내기 어려운, 손도 못대겠는 문제는 없었다.
구현이 조금 복잡한 문제는 있었는데, 평소에 개발과 코딩을 열심히 해왔다면 온몸을 비틀어서라도 풀 수 있을 것 같고, 복잡한 프로젝트 등등을 하며 변경에 유연한 구조 등을 고민했다면 한번쯤 겪어봤을 상황도 있었다.
js로 복잡한 비즈니스 로직을 개발해본 경험이 많고, 기본적인 자료구조와 알고리즘 문제를 풀 수 있는 실력이 있다면 통과할 것 같다.
4문제는 다 풀고, 2문제는 0.5만큼 풀고, 1문제는 시간이 없어서 손도 못대고 제출했다.

#### 리뷰

제대로 못 푼 문제 두 문제(0.5솔, 손도 못댄 문제)가 복잡한 구현보다는 알고리즘 문제에 가까워서 알고리즘 연습을 조금 더 해야 할 것 같다.
또다른 0.5솔 문제는 노드의 기능 중 하나를 사용하여 푸는 문제였는데, 프로젝트에서 겪을 수 있는 상황이기도 하지만 콜백 사용이 익숙하지가 않아서 제대로 못 풀었다.

요즘 취업 시장이 한파이고 토스 공채에 실력있는 개발자가 많이 지원했을 것 같아 아무 생각 안하고 개발하면서 결과를 기다렸다.
결과는 통과했고, 과제 테스트를 보게 되었다.

## 과제 테스트

과제 테스트는 이틀 동안 주어진 요구사항을 구현하는 테스트였다.
자세한 사항은 말할 수 없으나, 과제 테스트의 요구사항은 프로젝트를 하며 한번쯤 해볼만한 기능이라고 생각한다.
1일차엔 요구사항을 분석하고 어떻게 구현할 지 생각하고 서치하며 먼저 구현을 하는데에 초점을 두었다.
2일차엔 미처 구현하지 못한 요구사항을 마저 구현하고 리팩토링을 하였다.
시간이 부족하여 리팩토링을 다 하지는 못했고 테스트 코드도 정말 하찮게 썼지만, 일단 시간이 다되어 제출하였다.

과제 테스트를 개발할 때에는 아래 우선순위로 했었다.

1. 요구사항을 모두 구현한다.
2. 변경에 유연한 구조로 만든다.
3. 리소스를 효율적으로 사용하는 구조로 만든다.

변경에 유연한 구조로 만들기 위해 객체지향적으로 만드려 했고, 헤드 퍼스트 디자인 패턴 책을 좀 뒤적거렸다.
리소스를 효율적으로 사용하게 하기 위해 요구사항 명세서에 명시되지 않은 극한 상황을 가정하고, 더 효율적으로 동작하기 위해 어떤 구조로 가야 할 지 고민했었다.

#### 리뷰

아쉬웠던 부분은,

1. 디자인 패턴이 완벽히 적용되지 않았다
2. 함수 하나가 너무 많은 일을 한다
3. 함수가 크다 보니 테스트가 조악하다
4. 요구사항을 구현하는 데에 best practice와 좀 먼 것 같다
5. 에러 처리가 미숙하다
6. 스트림 처리를 하고 싶었으나 잘 몰라서 적용 못했다

테스트 종료 시간이 되었을 때 만족스러운 결과가 나오진 않았지만, 일단은 제출하고 그 뒤에도 좀 더 고민하고 찾아보던 중이었다.

## 이력서와 포폴

솔직히 과제 테스트를 만족스럽게 제출하진 못했지만, 왠지 모르게 기술 면접에 갈 수도 있겠다는 생각이 들었다.
과제 테스트를 진행하며 고민도 많이 했었고, 그것이 코드로 보이도록 하려고 노력했으니, 조금은 희망을 가져보고 싶은 마음이었다.
그래도 떨어지면 내 실력이 부족한 탓이니 더 정진하면 되겠다고 마음을 가다듬었다.

그리고 과제 테스트 결과가 나오는 날, 두근두근 메일을 열었더니.. 통과였다.
이쯤 되니 더 잘하고 싶은 마음도 생기고, 기술 면접에서 내가 어느 만큼의 퍼포먼스를 낼 수 있는지도 궁금했다.

지금까지 토스 NEXT 채용 과정을 진행하며 이력서와 포트폴리오를 내지 않았는데, 기술 면접을 앞두고 이력서와 포트폴리오를 내야 했다.
개인적으로 토스가 운영하는 [오픈소스](https://github.com/toss/nestjs-aop)에 기여할 수 있는 부분이 생겨 기여를 마무리 짓고 기존에 작성했던 이력서와 포트폴리오를 주변 개발자들의 피드백을 받아서 수정하여 제출했다.
이력서에는 인적사항과 프로젝트의 간단한 성과 위주로 작성했고, 포폴은 프로젝트에 있었던 문제 상황과 해결 방법, 성과에 대해 자세히 설명하고 이해를 돕기 위한 그림과 사진 등을 첨부하였다.

그렇게 밤새서 이력서랑 포폴을 만들고 제출하고, 기술 면접까지 끊임없는 자기 회고에 들어갔다..

## 기술 면접

기술 면접 준비는 일단 인터넷에 있는 토스 면접 후기를 검색하기도 하고, 주위 탐문을 하며 정보를 좀 얻었다.

그리고 낸 결론은,

1. 주로 이력서 상의 프로젝트에 관한 면접
2. 과제 테스트가 있었으니 과제 테스트 리뷰도 할 것
3. 맥락없는 CS 지식 질문은 없을 것 같고, 이력서나 과제 테스트 리뷰 맥락에서 CS 질문이 들어올 것
4. 꼬리 질문이 많이 들어올 테니 이력서/과제 테스트에서 결정을 내릴 때 한 고민을 잘 정리하자

로 정리했다.

#### 준비

그렇게 이력서 상의 프로젝트에 대해 내가 쓴 기술을 다시 찾아서 공부하고, 내가 결정을 내릴 때 당시의 상황을 정리하고 했던 고민들을 떠올리는 시간을 무한으로 즐겼다.
특히 어떤 기술을 쓰거나 어떤 문제를 어떻게 풀었는지 설명할 수 있는 이유를 찾는 데에 집중했고, 평소에도 고민과 결정을 내릴 때에 인기 많으니까, 힙해 보이니까 대신 나름대로 납득할 수 있는 이유를 찾아서 결정을 내렸던 것이 도움이 많이 되었던 것 같다.
그래도 문제를 해결하고 기술을 선택할 때 블로깅 등을 통해 정리했다면 이 과정이 좀 더 쉬웠을 것 같다.

과제 테스트 준비는 과제 테스트 끝나고 결과 기다리는 동안 정리했던 아쉬웠던 부분과 그것을 어떻게 개선할 지 리팩토링도 해보고 서치하며 준비했다.
이력서와 마찬가지로 어떤 고민을 하고 설계하고 어떤 생각으로 코드를 그렇게 짰는지 설명할 수 있게 연습하며 준비했었다.

역질문 시간은 토스 SLASH 2023 컨퍼런스를 보며 느낀 점과 노드/WA 챕터의 특징 등에 대해 궁금한 점 등을 질문으로 준비했다.

#### 기술 면접

면접이 시작되고, 면접관 2분이 들어오셔서 예상대로 과제 테스트 리뷰와 이력서 리뷰를 진행했다.
면접 분위기는 면접관들이 긴장도 많이 풀어주시고, 코드 리뷰 + 아키텍처 리뷰를 진행하는 느낌으로 편안하게 대화하는 기분이었다.
어떤 발생 가능한 상황에 대해서 어떻게 풀어나갈지 등을 많이 진행했고, 조금 대답이 막히면 힌트도 주셔서 어찌저찌 대답할 수 있었다.
과제 테스트에서 내가 아쉽게 느꼈던 부분 이외에도 많은 부분을 리뷰했고, 솔직히 말하자면 내 개발/코딩 실력이 많이 부끄러웠다...
그 후엔 이력서 리뷰를 진행했는데, 토스 오픈소스에 기여한 경험과 몇 가지 이력서에 적어놓은 부분에 대해 설명하였다.
잘 모르는 부분에 대해서 질문이 들어왔을 땐, 잘 모르는 부분이라 먼저 말하고 아는 부분까지 설명하였다.

#### 리뷰

어찌저찌 역질문 시간까지 마치고 들었던 생각은, 꽤 즐거운 경험이었다는 것이였다.
내 부족한 부분을 많이 확인하기도 했고, 현업에 종사하는 엔지니어와 코드 리뷰와 아키텍처 리뷰를 하는 것이 꽤 재밌었다.
평소에 개발 얘기를 많이 하고 컨퍼런스와 기술 블로그를 찾아보았던 것, 여러 상황을 가정하고 어떤 설계를 가져가고 코드를 어떻게 짤 지 고민해보는 경험들 등이 기술 면접에 좋게 작용한 것 같다.

아쉬웠던 점은 면접관이 하는 질문의 요지를 파악하지 못하고 가끔씩 헤멘 부분과, 무엇 하나를 설명해도 조금은 장황하게 설명한 것 같다.
앞으로는 질문의 의도를 정확히 파악해서 간단하고 명료하게 대답/설명하는 연습을 해야겠다.

## 문화 적합성 면접

기술 면접의 막바지에서, 면접관 분들에게서 긍정적인 느낌을 많이 받았다.
떨어지더라도 내가 부족한 부분을 확인했기 때문에 보완해서 더 나아지면 된다는 마음으로 기다렸다.

면접 본 다음날 전화로 기술 면접 통과 및 문화 적합성 면접 날짜를 잡고 많이 기뻤다.
기쁜 마음도 조금만 즐기고 접어두고, 토스 피드와 유튜브, 아티클 등등을 정독했다.
이전에 읽거나 봤던 것도 몇개 있긴 했지만 다시 보면서 토스 기업 문화를 확인했고, 나는 어떤 사람인지 지금까지 내린 결정들과 생각들을 다시 정리하기도 하였다.

#### 준비

내가 문화 적합성 면접을 준비하며 세운 전략은,

1. 나를 솔직하게 보여주자.
2. 내가 토스라는 기업과 잘 맞는다는 걸 어필하자.

이 두가지 였다.

첫째는 다양한 후기들에도 나와있기도 하고, 컬쳐 핏이라는 판단하기 애매하고 주관적인 평가 기준에 적어도 솔직하기라도 해야 판단하기 쉬울 것 같아서였다.
거짓말을 네이티브 수준으로 구사하는 것이 아니면 오래 대화를 나누면 대강 들통나게 되있다.
둘째는 나 스스로 토스의 기업 문화와 어울린다고 예전부터 생각했기 때문이다.
토스 기업 문화하면 사람들이 많이 떠올리는 것은 [일이 빡세고 힘든 대신 보상이 좋다], [토양어선, 역삼의 등대] 등등.. 이지만, 난 사실 보상이 좋으면 일이 많고 힘든 건 당연하다고 생각한다.
그리고 나 자신이 쉬운 일, 적당히 하면서 적당히 사는 것 등을 지향하지 않는다.
나는 좀 힘들고 어렵더라도 성취감을 느낄 수 있고, 하고 싶고, 재밌어하는 일을 하려는 사람이다.
이렇게 생각하고 준비하며, 문화 적합성 인터뷰를 시작하게 되었다.

#### 컬쳐핏 면접

면접관과 1시간 반 가량 대화를 나누며, 내가 지금까지 어떤 생각으로 인생의 결정을 내렸고 방향을 잡아왔으며 내가 생각하는 방식과 가치관에 대해 얘기하였다.
이전에 인성 혹은 컬쳐핏 면접을 보지는 않았지만, 질문의 스펙트럼이 다른 인성/컬쳐핏 면접의 스펙트럼을 벗어나진 않았다고 생각한다.
1번 전략에 따라 나 자신이 생각하는 단점도 많이 얘기하였고 2번 전략처럼 토스와 내가 잘 맞는다고 생각하는 점도 많이 얘기하였다.

면접이 끝나고 느낀 점은, 정말 솔직하게 많이 얘기했다는 기분이었다.
그러나 긍정적인 느낌은 없었다. 결과는 3일 후에 메일이 왔고, **불합격**이었다.

#### 리뷰

컬쳐 핏 면접에서 아쉬웠던 부분은,

1. 전략의 선정과 우선순위가 잘못되었다. 내가 토스라는 기업과 잘 맞는다고 해도, 그건 내 자신의 관점이지 토스가 날 뽑아야 할 이유가 되진 않는다. 토스와 내가 어떤 시너지를 낼 수 있을지 더 고민해보고 그것을 어필했어야 하는데, 단지 '난 잘 맞을 것 같아요' 라고만 말하는 사람을 뽑을 이유가 있을까?
2. 부정적인 면에서 너무 솔직했던 것 같다. 내가 생각하는 단점이 줄줄이 말하지 않아도 어차피 대화하며 단점이라고 생각할 부분은 보일텐데.. 부정적인 느낌(No signal)을 너무 보인 것 같다.
3. 전체적으로 준비가 많이 부족했다. 토스는 컬쳐핏 면접에서 많이 떨어진다는 얘기를 듣기도 했지만, 애초에 내가 컬쳐 핏이 잘 맞는다고 생각하기도 했기에 딱히 준비 안하고 나 자신을 보여주자 마인드로 갔다. 하지만 면접관은 내가 초면이고, 컬쳐 핏 면접도 결국 내가 토스에 왜 필요한지 어필하는 시간이어야 한다. 다음 컬쳐핏 면접부터는 대충 마인드는 버리고 심기일전 해야겠다.

## 토스 NEXT를 마치고 나서

토스 NEXT 공채를 통해서 운 좋게 코딩 테스트, 과제 테스트, 기술 면접까지 통과했지만 마지막 단계인 문화 적합성에서 떨어지고 나니 많이 슬펐다..
아직 이력서를 여기저기 넣고 다닌 것도 아니고 취준 경력이 오래된 것도 아니지만, 마지막 단계에서 떨어지는 건 타격이 꽤 크다는 것을 느꼈다.

전체적으로 토스 채용 과정은 긍정적이었다.
코딩 테스트는 그다지 좋아하지 않는 어려운 알고리즘 문제 보다는 실무에서 마주칠 만한 상황의 구현 문제 + 적당한 난이도의 알고리즘 문제로 구성되었다.
과제 테스트 또한 내 고민과 역량을 잘 보여줄 수 있는 주제로, 난이도에 알맞은 충분한 시간을 두고 출제되었다.
기술 면접은 압박 분위기가 없는 편안한 상태에서 과제 리뷰와 이력서 리뷰, 문제 상황에 대한 해결책을 찾아나가는 방식의 대화 등이 즐겁게 느껴졌다.

문화 적합성 면접은 아쉬움이 많이 남았다. 내가 어필을 못한 부분, 열정을 보여주지 못한 부분이 많은 것 같다.
이번 탈락을 계기로 나에 대해 더 돌아보고 앞으로 더 나아갈 방향과 힘을 얻었고, 더 정진해야겠다.

이제 다양한 기업들에 이력서를 제출하고 채용 시장을 더 경험해볼 계획이다.
실패를 해야 성공하는 법도 배운다는 말도 있으니, 계속 열심히 하자! 아자아자!
