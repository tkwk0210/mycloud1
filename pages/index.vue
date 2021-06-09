<template>
  <div>
    <section class="hero is-primary">
      <div class="hero-body">
          <p class="title"><i class="fas fa-chess"></i>
           Chess Game
          </p>
          <p class="subtitle">
            체스 게임에 대해 소개 해드립니다.
          </p>
      </div>
    </section>

    <div class="columns">
      
      <article class="notification is-warning is-light">
        <div class="notification is-warning is-light-header">
          <p> 체스 규칙 </p>
        </div>

        <div class="notification is-warning is-light-body">
          <figure class="image is-128x128">
            <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/d/d9/Opening_chess_position_from_black_side.jpg/200px-Opening_chess_position_from_black_side.jpg" 
            alt="">
          </figure>
          
          <p>
            경기준비 <br>
            <br>1. 체스는 가로 8칸(랭크는 가로 1부터 8), 세로 8줄(파일은 세로 a 부터 h)로 된 사각형 보드로 플레이한다. 64칸의 색상은 밝은 칸(light squares)과 어두운 칸(dark squares)으로 나뉜다. 
            <br>2. 보드는 각 플레이어의 왼쪽에서 가까운 랭크의 어두운 칸(dark squares)이 오도록 해야하고 퀸은 플레이어의 색상에 맞게 위치한다. 피스는 화이트와 블랙으로 나뉜다. 
            <br>3. 플레이어는 화이트와 블랙으로 각각 16개의 피스를 갖고 게임을 시작한다. 1개의 킹, 퀸 2개의 룩, 비숍과 나이트, 8개의 폰으로 구성되어있다.
          </p>
        </div>
      </article>

      <article class="notification is-warning is-light">
        <div class="notification is-warning is-light-header">
          <p>행마법</p>
        </div>
        <div class="notification is-warning is-light-body">
          <p>
            항상 화이트가 먼저 이동한다. 플레이어는 번갈아가면서 1개의 피스를 이동해야된다. 피스를 잡으면 그 피스를 움직여야 한다.(캐슬링은 제외) 피스를 잡으면 보드 그 피스를 움직인다.앙파상을 제외하고 상대의 피스의 칸으로 이동해서 상대의 피스를 잡는다. 킹이 움직일 수 없는 경우 게임은 끝이 난다. 그것은 체크메이트 또는 스테일메이트 중 하나다.
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