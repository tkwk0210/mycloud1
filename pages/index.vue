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
          
          <th> 경기준비 </th> <br>
          <br>1. 체스는 가로 8칸(랭크는 가로 1부터 8), 세로 8줄(파일은 세로 a 부터 h)로 된 사각형 보드로 플레이한다. 64칸의 색상은 밝은 칸(light squares)과 어두운 칸(dark squares)으로 나뉜다. 
          <br>2. 보드는 각 플레이어의 왼쪽에서 가까운 랭크의 어두운 칸(dark squares)이 오도록 해야하고 퀸은 플레이어의 색상에 맞게 위치한다. 피스는 화이트와 블랙으로 나뉜다. 
          <br>3. 플레이어는 화이트와 블랙으로 각각 16개의 피스를 갖고 게임을 시작한다. 1개의 킹, 퀸 2개의 룩, 비숍과 나이트, 8개의 폰으로 구성되어있다.
          <br><br>
          
          <li> <nuxt-link to="/chesspieces">체스 기물</nuxt-link></li><br>
          <li> <nuxt-link to="/chessopening">체스 오프닝</nuxt-link> </li><br>
          <li> <nuxt-link to="/chessnotation">체스 기본법</nuxt-link> </li><br>
          <li> <nuxt-link to="/chesstactics">체스 전술</nuxt-link> </li>

          <br><br>
          <th> 경기 종료 </th>
          체크메이트, 스테일메이트, 리사인(Resign), 50수 무승부, 쓰리폴드 레피티션이 됐을때 게임은 끝이난다.
        </div>
      </article>

    </div>
  </div>
</template>