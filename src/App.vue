<template>
  <div id="app" class="animation-blur-load">
    <router-view></router-view>
    <footer id="main-layout">
      <div>
        <p class="right">
          ©若林稔弥・講談社／徒然チルドレン製作委員会
        </p>
        <ul class="banner unstyled">
          <li>
            <a href="http://tsuredurechildren.com/" target="_blank" class="">
              <img src="http://tsuredure-project.jp/img/banner_1.png" alt="徒然チルドレン" height="16" class="">
            </a>
          </li>
          <li>
            <a href="http://www.kodansha.co.jp/" target="_blank">
              <img src="http://tsuredure-project.jp/img/banner_2.png" alt="講談社" height="16">
            </a>
          </li>
          <li>
            <a href="http://www.kingrecords.co.jp/cs/default.aspx" target="_blank">
              <img src="http://tsuredure-project.jp/img/banner_3.png" alt="KING RECORDS" height="16">
            </a>
          </li>
          <li>
            <a href="http://www.shonenmagazine.com/" target="_blank" class="">
              <img src="http://tsuredure-project.jp/img/banner_4.png" alt="マガジン" height="16" class="">
            </a>
          </li>
        </ul>
      </div>
    </footer>
    <footer id="sub-layout">
      <div>
        <div class="ts stackable horizontal list">
          <div class="item">
            <a href="http://tsuredurechildren.com/" target="_blank" class="">
              <img src="http://tsuredure-project.jp/img/banner_1.png" alt="徒然チルドレン" height="16" class="">
            </a>
          </div>
          <div class="item">
            <a href="http://www.kingrecords.co.jp/cs/default.aspx" target="_blank">
              <img src="http://tsuredure-project.jp/img/banner_3.png" alt="KING RECORDS" height="16">
            </a>
          </div>
        </div>
        <div class="ts stackable horizontal list">
          <div class="item">
            <a href="http://www.kodansha.co.jp/" target="_blank">
              <img src="http://tsuredure-project.jp/img/banner_2.png" alt="講談社" height="16">
            </a>
          </div>
          <div class="item">
            <a href="http://www.shonenmagazine.com/" target="_blank" class="">
              <img src="http://tsuredure-project.jp/img/banner_4.png" alt="マガジン" height="16" class="">
            </a>
          </div>
        </div>
         <div style="clear:both;"></div> 
         <p class="right">
          ©若林稔弥・講談社／徒然チルドレン製作委員会
        </p> 
      </div>
    </footer>
  </div>
</template>

<script>
export default {
  name: 'app'
}
</script>

<style>
@import url(./components/Home_m.css);
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

.animation-blur-load {
  animation-name: blur-load;
  animation-duration: 1s;
  animation-timing-function: linear;
}

@keyframes blur-load {
  0% {
    opacity: 0;
  }
  100% {
    opacity: 1;
    filter: blur(1px);
  }
}

footer {
  position: relative;
  bottom: 0;
  width: 100%;
  height: 33px;
  background-color: #26bc9b;
}

footer .right {
  font-size: 10px;
  color: white;
  line-height: 33px;
  float: left;
  margin-left: 220px;
}

footer .banner {
  padding-top: 7px;
  float: right;
  height: 19px;
  margin-right: 100px;
}

footer li {
  display: inline;
}
</style>
