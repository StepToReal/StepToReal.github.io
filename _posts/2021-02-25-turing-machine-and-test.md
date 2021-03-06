---
title: "튜링 머신 이해"
last_modified_at: 2021-02-25T00:30:00
toc: true
---
튜링 머신 이해

영화 "이미테이션 게임"을 보면 2차 세계대전 당시 독일의 애니그마 암호를 해독하기 위해 거대한 기계를 만드는 장면이 나온다. 튜링 머신을 얼핏 들어본 사람들은 영화에 나온 기계가 튜링 머신인줄 잘못 알고있는 사람들도 있을 것이다. 나도 처음 이 영화를 봤을때는 영화에 나온 기계가 튜링머신인 줄 알았다. 알아보니 튜링 머신은 실존하는 기계장치가 아니었다. 그럼 대체 튜링머신은 무엇일까??

튜링 머신은 앨런 튜링이 1933년에 발표한 논문 "On computerble numbers, with an application to the Entscheidungsproblem." 에 나온 내용으로 모든 계산이 가능한 가상의 기계(머신)이다. 잠시 삼천포로 빠지면... 논문의 제목에 계산 가능한 이란 뜻으로 "On computerble"을 사용했는데 이때 튜링이 Computerble 이라는 단어를 사용함으로써 현재 컴퓨터가 컴퓨터로 불리게 됐다는 얘기가 있다.

해당 논문은 다비트 힐베르트의 힐베르트 프로젝트가 성립할 수 없음을 증명한 것인데 힐베르트 프로젝트는 정의와 공리를 입력하면 모든 수학적 정리를 도출할 수 있는 기계를 만드는 것이었다. 앨런 튜링은 모든 계산이 가능한 가상의 머신(튜링 머신)을 설계해 놓고 이 기계가 풀수 없는 문제가 있음을 증명하여 힐베르트 프로젝트가 불가능한 것임을 증명 하였다.

여기서 중요한 점은 모든 계산이 가능한 가상의 머신이다. 이 머신이 훗날 튜링 머신으로 불리게 되었고 현대 컴퓨터의 원형이 된다. 튜링 머신은 4가지 구성요소를 갖는다.

> 1. 테이프: 정보를 기록할 수 있으며 무한한 길이를 갖는다.
> 2. 기호집합: 테이프에 기록 될 수 있는 기호 집합
> 3. 헤드: 현재 위치한 셀을 읽고 쓸수 있고 좌, 우로 이동 가능.
> 4. 상태: 튜링 머신이 가질 수 있는 상태 집합   

튜링머신의 핵심은 무한한 길이를 갖는 테이프와 무한히 가질 수 있는 상태집합 인 것 같다. 현대 컴퓨터는 메모리 및 CPU의 제한이 있기 때문에 이론적으로 제한이 없는 튜링머신이 훨씬 더 많은 일을 수행 할 수 있다. "튜링 컴퓨터블 하다" 라는 말이 모든 계산을 수행할 정도의 성능을 만족한다는 뜻으로 쓰이기도 한다고 한다.

위 4가지 구성요소를 가지고 명령테이블을 만들어 수행이 가능한데 간단한 예제 명령 테이블과 그에따른 실행 예제는 아래와 같다.

    **그림 넣기..

튜링 머신의 개념을 확장해서 UTM (Universal Turing Machine) 이라는 개념이 있다. UTM은 어떤 튜링머신도 따라할 수 있는 범용의 튜링 머신으로 n개의 튜링 머신이 있을 때 명령테이블을 확인해서 n개의 튜링머신을 가상으로 실행해 볼 수 있는 기계를 뜻한다. 해당 구조는 폰노이만에 의해 현대 컴퓨터의 구조로 발전하게 된다.

    **그림 넣기..

마무리 하자면.. 튜링 머신은 하나의 기능을 처리하는 응용프로그램이고 UTM이 여러 응용프로그램을 실행 시키는 운영체제인 샘이다. 영화에 나온 크리스토퍼는 (기계 이름이다.) 튜링 머신의 개념을 바탕으로 만들어 졌으나 엄밀히 말해 무한한 테이프와 무한한 상태를 갖을 수 없기 때문에 튜링 머신은 아니며 애니그마 해독이라는 한 가지 일만 수행 할 수 있으므로 현대 컴퓨터로 치자면 응용프로그램을 기계로 만들었다 정도로 볼 수 있을 것 같다. 앨런 튜링은 무한대의 상태와 저장공간을 가질 수 있는 튜링 머신이 있고 인간이 생각하는대로 동작하게 할 수 있다면 인공지능이 가능 할 것이라고 최초로 주장했다고 한다.