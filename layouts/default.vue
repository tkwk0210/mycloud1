<template>
  <div>
    <nav class= "breadcrumb">
      <ul>
        <li> <nuxt-link to="/"><i class="fas fa-home"></i> 홈으로 </nuxt-link> </li>
        <li> <nuxt-link to="/chesspieces">기물</nuxt-link></li>
        <li> <nuxt-link to="/chessopening">체스 오프닝</nuxt-link> </li>
        <li> <nuxt-link to="/chessnotation">체스 기본법</nuxt-link> </li>
        <li> <nuxt-link to="/chesstactics">체스 전술</nuxt-link> </li>
      </ul>
    </nav>
    <nuxt/>

    <footer class="footer">
      <div class="content has-text-centered">
        2021- 체스에 대해서 알아보자
      </div>
    </footer>
  </div>
</template>

<style>
html {
  font-family: "Source Sans Pro", -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif;
  font-size: 16px;
  word-spacing: 1px;
  -ms-text-size-adjust: 100%;
  -webkit-text-size-adjust: 100%;
  -moz-osx-font-smoothing: grayscale;
  -webkit-font-smoothing: antialiased;
  box-sizing: border-box;
}

*, *:before, *:after {
  box-sizing: border-box;
  margin: 0;
}

.button--green {
  display: inline-block;
  border-radius: 4px;
  border: 1px solid #3b8070;
  color: #3b8070;
  text-decoration: none;
  padding: 10px 30px;
}

.button--green:hover {
  color: #fff;
  background-color: #3b8070;
}

.button--grey {
  display: inline-block;
  border-radius: 4px;
  border: 1px solid #35495e;
  color: #35495e;
  text-decoration: none;
  padding: 10px 30px;
  margin-left: 15px;
}

.button--grey:hover {
  color: #fff;
  background-color: #35495e;
}
</style>

