<template>
  <div>
    <section class="hero is-primary">
      <div class="hero-body">
          <p class="title"><i class="fas fa-chess"></i>
           체스 기본법
          </p>
          <p class="subtitle">
            체스 기본법에 대해 알아보자
          </p>
      </div>
    </section>
    <div class = "cloumns">
        <article class="notification is-warning is-light">
            <div class="notification is-warning is-light-header">
                <th>체스 표기법(Chess notation)</th>
            </div>
            <div class="notification is-warning is-light-body">
                <tbody>
                    가장 널리 쓰이며 체스판의 좌표를 문자와 숫자를 이용해 표기한다.
                    <br>기물들은 대문자로 다음과 같이 표기한다.
                    <br>K: 킹 (King)
                    <br>Q: 퀸 (Queen)
                    <br>R: 룩 (Rook)
                    <br>B: 비숍 (Bishop)
                    <br>N: 나이트 (Knight)
                    <br>P: 폰 (Pawn; 일반적으로 표기하지 않고 생략한다.)
                    <br>기물의 위치는 세로줄, 가로줄 순으로 표기된다. 예로 우측 그림에서 킹은 e8에 있다.
                    <br>2개의 기물이 같은 칸으로 이동이 가능한 특수한 경우에는 문자 혹은 숫자를 추가하여 이동하는 기물이 어디에 있었는지를 나타낸다. 예를 들어 f3로 갈 수 있는 나이트가 2개이고, 하나의 나이트는 g열에, 또 다른 하나는 h열에 있었다고 했을 때, g열에 있는 나이트가 f3로 이동하면 Ngf3로 표기한다.
                    <br>기물을 잡을 경우엔 가운데 "x"를 표기한다. Bxf3는 비숍이 f3에 있는 기물을 잡았다는 것을 의미한다. e열에 있는 폰이 d5에 기물을 잡은 경우 exd5 또는 exd로 표기한다.
                    <br>폰이 마지막 랭크로 이동해서 프로모션을 할 경우 e1Q 또는 e1=Q로 표기한다. 캐슬링을 할 경우 킹사이드 캐슬링은 0-0, 퀸사이드 캐슬링은 0-0-0으로 표기한다.(숫자 0) 폰이 앙파상으로 폰을 잡을 경우 동일하게 표기하지만 앙파상으로 잡은 것인지 일반 행마로 잡은 것인지 구분하기 위하여 "e.p." 등으로 표기한다. 상대의 킹을 체크 할 경우엔 "+"로 표기한다. 체크메이트를 했을 경우 "#"으로 표기한다. ("++"은 더블 체크다.) 게임이 끝나고 화이트가 이겼을 경우 "1-0" 블랙이 이겼을 경우 "0-1"로 무승부일 경우 "½–½"로 표기한다.
                    <br>각 수의 대한 주석은 구두점을 이용한다. "!" 좋은 수, "!!" 아주 좋은수, "?" 실수, "??" 블런더, "!?" 괜찮은수, "?!" 의심이 가는수로 표기한다.
                </tbody>
            </div>
                <div class="notification is-warning is-light-header">
                    <th>목적</th>   
                </div>
                <div class="notification is-warning is-light-body">
                    <tbody>
                        체스 표기법(Chess notation)은 체스 기물의 움직임을 기록하기 위해 만들어진 것이다.
                    </tbody>
                </div>
        </article>
    </div>
    <article class="notification is-warning is-light">
        
        <div class="notification is-warning is-light-header">
            <th>추가적...</th>
        </div>
        <div class="notification is-warning is-light-body">
            <th>확장 대수 표기법</th>
                <br>원래위치-새위치로 나타낸다. 캐슬링과 프로모션은 위의 방식을 사용한다.<br>

            <br><th>ICCF 숫자 표기법</th>
                <br>숫자만을 사용한 표기법이다. 움직임은 세로줄 뒤에 열을 나타내며, 세로줄의 번호와 가로줄 모두 1,2,3 순이다. 
                <br>백의 백퀸쪽 룩의 11부터 흑의 흑킹쪽 룩 88번까지로 표기된다. 백이 처음 e폰을 2칸 움직인 것은 5254로 표기한다. 
                <br>캐슬링은 킹이 두칸을 움직인것으로 표현하며, 프로모션은 5번째 칸에 승진한 기물을 숫자로 표기한다. 
                <br>(1=퀸, 2=룩, 3=비숍, 4=나이트)<br>

            <br><th>서술 표기법</th>
                <br>과거에 주로 사용되던 표기법으로, 체스판의 파일을 기물 이름으로 표기한다. 
                <br>예를 들어, c열은 QB 로 표기하는데, '퀸 쪽 비숍 열'이라는 뜻이다. 행은 각 플레이어의 관점에서 표기한다. 
                <br>일례로 백의 QB3는 흑의 QB6이다. 바비피셔의 유명한 저서 my 60 memorable games 가 서술 표기법으로 기보가 작성되어있다.

        </div>
    </article>
  </div>
</template>