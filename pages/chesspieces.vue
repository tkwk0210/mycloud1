<template>
  <div>
    <section class="hero is-primary">
      <div class="hero-body">
          <p class="title"><i class="fas fa-chess"></i>
           기물
          </p>
          <p class="subtitle">
            체스 기물에 대해 알아보자.
          </p>
      </div>
    </section>

    <div class="columns">
      <article class="notification is-warning is-light">
        <div class="notification is-warning is-light-header">
          <p>행마법</p>
        </div>
        <div class="notification is-warning is-light-body">
          <p>
            항상 화이트가 먼저 이동한다. 플레이어는 번갈아가면서 1개의 피스를 이동해야된다. 
            <br>피스를 잡으면 그 피스를 움직여야 한다.(캐슬링은 제외) 피스를 잡으면 보드 그 피스를 움직인다.
            <br>앙파상을 제외하고 상대의 피스의 칸으로 이동해서 상대의 피스를 잡는다. 킹이 움직일 수 없는 경우 게임은 끝이 난다. 
            <br>그것은 체크메이트 또는 스테일메이트 중 하나다.
            <br> 각 피스는 이동의 특징이 있다. 아래의 보드에서 점은 다른 피스가 초기상태와 목적지 사이의 칸에 없는 경우 피스가 이동 할 수 있는 칸을 표시한다.
            <br>
            <table class="table is-fullwidth">
              <thead>
                <th>기물</th>
                
                <th>이동 방식</th>
              </thead>

              <tbody>
                <tr>
                  <td><i class="fas fa-chess-pawn"></i>폰 </td>

                  <td>초기상태에서 한 칸 혹은 두 칸을 전진할 수 있고 한 번 움직인 이상 하나씩만 전진할 수 있으며, 후퇴가 불가능하다(한국식 장기의 졸(卒)과 유사). 상대방의 피스는 대각선 한 칸으로만 잡을 수 있다. 특별한 움직임으로 프로모션과 앙파상이 있다.</td>
                </tr>
                <tr>
                  <td><i class="fas fa-chess-rook"></i>룩</td>
                  <td>전후와 좌우로 칸 수의 제한 없이 움직일 수 있다(한국식 장기의 차(車)와 같음). 룩은 킹이 캐슬링할때 필요하다.</td>
                </tr>
                <tr>
                    <td><i class="fas fa-chess-bishop"></i>비숍</td>
                    <td>대각선 방향으로 칸 수의 제한 없이 움직일 수 있다. 어두운 칸 비숍, 밝은 칸 비숍은 자기의 색의 칸에서만 이동이 가능하다.</td>
                </tr>
                <tr>
                  <td> <i class="fas fa-chess-knight"></i>나이트 </td>
                  <td>두 칸 전진한 상태에서 좌우로 한 칸 움직일 수 있다(한국식 장기의 마(馬)와 같음). 피스들 중에서 유일하게 다른 피스를 뛰어넘을 수 있다.</td>
                </tr>
                <tr>
                  <td><i class="fas fa-chess-queen"></i>퀸</td>
                  <td>전후좌우, 대각선으로 칸수 제한 없이 움직일 수 있다. 룩과 비숍의 기능을 합쳐 놓은 것으로 다방면으로 칸수 제한 없이 움직일 수 있어 피스 중 가장 강력하다고 할 수 있다.</td>
                </tr>
                <tr>
                  <td><i class="fas fa-chess-king"></i>킹</td>
                  <td>전후좌우, 대각선으로 한 칸씩 움직일 수 있다. 룩과 캐슬링을 할 수 있다.</td> 
                </tr>
              </tbody>
            </table>
            <nuxt-link to="/chesstrick">행마법 자세히</nuxt-link>
          </p>
        </div>
      </article>
    </div>
  </div>
</template>