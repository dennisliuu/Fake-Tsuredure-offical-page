<template>
  <div id="app">
    <div v-if="showlightbox">
      <div class="lb">
        <div class="lb-overlay">
          <!-- background for lightbox -->
          <iframe width="560" height="315" src="https://www.youtube.com/embed/XaVHGIj3tzc?rel=0&autoplay=1" frameborder="0" allowfullscreen></iframe>
          <!-- main content of lightbox -->
          <div class="lb-close" @click="showlightbox=false">
            <span class="close hairline"></span>
          </div>
          <!-- close button -->
        </div>
        <!-- end overlay -->
      </div>
    </div>
  
    <div v-if="showsidenav">
      <div class="lb">
        <div class="lb-overlay">
          <!-- background for lightbox -->
          <div style="display: block">
                      <nav>
            <ul class="loaded unstyled">
              <li>
                <a href="" class="grow">
                  NEWS
                </a>
              </li>
              <li>
                <a href="" class="grow">
                  introduction
                </a>
              </li>
              <li>
                <a href="" class="grow">
                  staff/cast
                </a>
              </li>
              <li>
                <a href="" class="grow">
                  character
                </a>
              </li>
              <li>
                <a href="" class="grow">
                  onair
                </a>
              </li>
              <li>
                <a href="" class="grow">
                  story
                </a>
              </li>
              <li>
                <a href="" class="grow">
                  music
                </a>
              </li>
              <li>
                <a href="" class="grow">
                  comic
                </a>
              </li>
              <li>
                <a href="" class="grow">
                  goods
                </a>
              </li>
              <li>
                <a href="" class="grow">
                  special
                </a>
              </li>
            </ul>
          </nav>
          </div>
          <!-- main content of lightbox -->
          <div class="lb-close" @click="showsidenav=false">
            <span class="close hairline"></span>
          </div>
          <!-- close button -->
        </div>
        <!-- end overlay -->
      </div>
    </div>
  
    <div id="main-layout">
      <div class="ts column narrow container grid">
        <div class="two wide column">
          <div class="loaded-1">
            <span class="_1" style="right: 0"></span>
            <span class="_2" style="right: 50%"></span>
            <span class="_3" style="left: 0"></span>
          </div>
          <nav>
            <ul class="loaded unstyled fade-in">
              <li>
                <a href="" class="grow">
                  NEWS
                </a>
              </li>
              <li>
                <a href="" class="grow">
                  introduction
                </a>
              </li>
              <li>
                <a href="" class="grow">
                  staff/cast
                </a>
              </li>
              <li>
                <a href="" class="grow">
                  character
                </a>
              </li>
              <li>
                <a href="" class="grow">
                  onair
                </a>
              </li>
              <li>
                <a href="" class="grow">
                  story
                </a>
              </li>
              <li>
                <a href="" class="grow">
                  music
                </a>
              </li>
              <li>
                <a href="" class="grow">
                  comic
                </a>
              </li>
              <li>
                <a href="" class="grow">
                  goods
                </a>
              </li>
              <li>
                <a href="" class="grow">
                  special
                </a>
              </li>
            </ul>
          </nav>
          <div class="sns fade-in">
            <ul class="unstyled">
              <li>
                <a href="">
                  <img src="http://tsuredure-project.jp/img/sns_tw.png" onmouseover="this.src='http://tsuredure-project.jp/img/sns_tw_h.png'" onmouseout="this.src='http://tsuredure-project.jp/img/sns_tw.png'" style="width: 20px;">
                </a>
              </li>
              <li>
                <a href="">
                  <img src="http://tsuredure-project.jp/img/sns_fb.png" onmouseover="this.src='http://tsuredure-project.jp/img/sns_fb_h.png'" onmouseout="this.src='http://tsuredure-project.jp/img/sns_fb.png'" style="width: 8px">
                </a>
              </li>
              <li>
                <a href="">
                  <img src="http://tsuredure-project.jp/img/sns_line.png" onmouseover="this.src='http://tsuredure-project.jp/img/sns_line_h.png'" onmouseout="this.src='http://tsuredure-project.jp/img/sns_line.png'" style="width: 17px">
                </a>
              </li>
            </ul>
          </div>
        </div>
        <div class="twelve wide column">
          <img src="../assets/mainvisual_3.jpg" style="width: 650px">
        </div>
        <div class="two wide column fade-in">
          <p style="margin: 10px" <img src="http://tsuredure-project.jp/img/top_batch_onair_3.png" width="180">
          </p>
          <ul class="unstyled sub_content">
            <li>
              <a href="http://tsuredure-project.jp/archives/129">
                <img src="http://tsuredure-project.jp/wp-content/uploads/2017/06/top_banner_dvdinfo.png">
              </a>
            </li>
            <li>
              <a href="http://tsuredure-project.jp/?p=152">
                <img src="http://tsuredure-project.jp/wp-content/uploads/2017/06/top_banner_dvd.png">
              </a>
            </li>
            <li>
              <a href="http://tsuredure-project.jp/?p=86">
                <img src="http://tsuredure-project.jp/wp-content/uploads/2017/06/Twitter_banner_360x90.png">
              </a>
            </li>
            <li>
              <a href="#">
                <img src="http://tsuredure-project.jp/img/top_youtube_banner8.png" @click="showlightbox=true">
              </a>
            </li>
          </ul>
        </div>
      </div>
  
      <div class="ts four column centered grid content">
        <div class="column top_news">
          <h2>NEWS</h2>
          <div class="time">2017.7.4</div>
          <a href="http://tsuredure-project.jp/archives/194">「徒然チルドレン」本日7/4（火）放送スタート！</a>
          <p class="more_buttom">
            <a href="http://tsuredure-project.jp/news">more ></a>
            <!-- <router-link to="/news">more ></router-link> -->
          </p>
        </div>
        <div class="column top_twitter">
          <h2>Twitter</h2>
          <div class="tweet_wrap">
            <p>
              <a href="https://twitter.com/tsuredure_anime">
                【商品情報】コンテンツシードより「#徒然チルドレン」の缶バッジが全8種で登場
                <img draggable="false" class="emoji" alt="❤" src="https://s.w.org/images/core/emoji/2.2.1/svg/2764.svg" width="10px"> ＜8/25(金)発売予定＞カバンなどにもつけやすく、目立つこと間違いなし
                <img draggable="false" class="emoji" alt="❤" src="https://s.w.org/images/core/emoji/2.2.1/svg/2764.svg" width="10px">
                <img draggable="false" class="emoji" alt="❤" src="https://s.w.org/images/core/emoji/2.2.1/svg/2764.svg" width="10px">
                <span class="inner_link">https://t.co/m7ndOmo21U</span>
                #徒チル…
                <span class="inner_link">https://t.co/iVPJUnmY8a</span>
              </a>
            </p>
            <p>
              <a href="#"></a>
            </p>
            <p>
              <a href="#"></a>
            </p>
            <p>
              <a href="#"></a>
            </p>
            <p>
              <a href="#"></a>
            </p>
          </div>
  
        </div>
      </div>
    </div>
  
    <div id="sub-layout">
  
      <p id="g_nav_button" @click="showsidenav=true"></p>
  
      <img src="http://tsuredure-project.jp/img/logo_sp.png" style="width: 38%">
      <br />
      <br />
      <img src="../assets/mainvisual_3.jpg" style="width: 300px">
      <div class="batch-wrap">
        <p class="batch">
          <span class="sp_text">2017年7月4日（火）より放送スタート</span>
        </p>
      </div>
      <div class="content2">
        <div class="content2-container">
          <div class="top_news2">
            <h2>NEWS</h2>
            <!-- <p class="more_button2">
                        <a href="http://tsuredure-project.jp/news">more &gt;</a>
                      </p>  -->
            <div style="top: -15px">
              <time class="time2">2017.7.13</time>
              <h3>
                <a href="http://tsuredure-project.jp/archives/255">
                  「徒然チルドレン」のカンバッジが全8種で登場です！
                </a>
              </h3>
            </div>
          </div>
          <div class="top_twitter">
            <h2>Twitter</h2>
            <div class="tweet_wrap">
              <p>
                <a href="https://twitter.com/tsuredure_anime">
                  【商品情報】コンテンツシードより「#徒然チルドレン」の缶バッジが全8種で登場
                  <img draggable="false" class="emoji" alt="❤" src="https://s.w.org/images/core/emoji/2.2.1/svg/2764.svg" width="10px"> ＜8/25(金)発売予定＞カバンなどにもつけやすく、目立つこと間違いなし
                  <img draggable="false" class="emoji" alt="❤" src="https://s.w.org/images/core/emoji/2.2.1/svg/2764.svg" width="10px">
                  <img draggable="false" class="emoji" alt="❤" src="https://s.w.org/images/core/emoji/2.2.1/svg/2764.svg" width="10px">
                  <span class="inner_link">https://t.co/m7ndOmo21U</span>
                  #徒チル…
                  <span class="inner_link">https://t.co/iVPJUnmY8a</span>
                </a>
              </p>
            </div>
          </div>
        </div>
      </div>
  
      <div class="sub_content">
        <div class="youtube">
          <ul class="unstyled">
            <li>
              <a href="#">
                <img src="http://tsuredure-project.jp/img/top_youtube_banner8.png" @click="showlightbox=true">
              </a>
            </li>
          </ul>
        </div>
        <div class="top_banners">
          <ul class="unstyled">
            <li>
              <a href="http://tsuredure-project.jp/archives/129">
                <img src="http://tsuredure-project.jp/wp-content/uploads/2017/06/top_banner_dvdinfo.png">
              </a>
            </li>
            <li>
              <a href="http://tsuredure-project.jp/?p=152">
                <img src="http://tsuredure-project.jp/wp-content/uploads/2017/06/top_banner_dvd.png">
              </a>
            </li>
            <li>
              <a href="http://tsuredure-project.jp/?p=86">
                <img src="http://tsuredure-project.jp/wp-content/uploads/2017/06/Twitter_banner_360x90.png">
              </a>
            </li>
          </ul>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data () {
    return {
      showlightbox: false,
      showsidenav: false
    }
  }
}
</script>

<style>
@import url(./Home_m.css);

#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
  margin-top: 27px;
  min-width: 1024px;
}

.loaded-1 {
  width: 140px;
  height: 270px;
  background-repeat: no-repeat;
  background-image: url('http://tsuredure-project.jp/img/logo_t.png');
  background-size: 140px 270px;

  /* -webkit-animation: fade 1s 2.2s forwards;
  -moz-animation: fade 1s 2.2s forwards;
  -o-animation: fade 1s 2.2s forwards;
  animation: fade 1s 2.2s forwards; */
}

@keyframes fade {
  from {
    opacity: 0;
  }
  to {
    opacity: 1;
  }
}

.loaded-1 ._1,
.loaded-1 ._2,
.loaded-1 ._3 {
  position: absolute;
  top: 0;
  width: 1px;
  background-color: #a5a6a6;
  display: block;
  /* height: 100%; */
  /* opacity: 1 !important; */
}

.loaded-1 ._1 {
  -webkit-animation: imganim 1.5s 1.6s cubic-bezier(0.165, 0.84, 0.44, 1);
  -moz-animation: imganim 1.5s 1.6s cubic-bezier(0.165, 0.84, 0.44, 1);
  -o-animation: imganim 1.5s 1.6s cubic-bezier(0.165, 0.84, 0.44, 1);
  animation: imganim 1.5s 1.6s cubic-bezier(0.165, 0.84, 0.44, 1);

  -webkit-webkit-animation-fill-mode: forwards;
  -moz-webkit-animation-fill-mode: forwards;
  -ms-webkit-animation-fill-mode: forwards;
  -o-webkit-animation-fill-mode: forwards;
  animation-fill-mode: forwards;
}

.loaded-1 ._2 {
  -webkit-animation: imganim 1.5s 1.8s cubic-bezier(0.165, 0.84, 0.44, 1);
  -moz-animation: imganim 1.5s 1.8s cubic-bezier(0.165, 0.84, 0.44, 1);
  -o-animation: imganim 1.5s 1.8s cubic-bezier(0.165, 0.84, 0.44, 1);
  animation: imganim 1.5s 1.8s cubic-bezier(0.165, 0.84, 0.44, 1);

  -webkit-webkit-animation-fill-mode: forwards;
  -moz-webkit-animation-fill-mode: forwards;
  -ms-webkit-animation-fill-mode: forwards;
  -o-webkit-animation-fill-mode: forwards;
  animation-fill-mode: forwards;
}

.loaded-1 ._3 {
  -webkit-animation: imganim 1.5s 2s cubic-bezier(0.165, 0.84, 0.44, 1);
  -moz-animation: imganim 1.5s 2s cubic-bezier(0.165, 0.84, 0.44, 1);
  -o-animation: imganim 1.5s 2s cubic-bezier(0.165, 0.84, 0.44, 1);
  animation: imganim 1.5s 2s cubic-bezier(0.165, 0.84, 0.44, 1);

  -webkit-webkit-animation-fill-mode: forwards;
  -moz-webkit-animation-fill-mode: forwards;
  -ms-webkit-animation-fill-mode: forwards;
  -o-webkit-animation-fill-mode: forwards;
  animation-fill-mode: forwards;
}

@keyframes imganim {
  from {
    height: 0;
  }
  to {
    height: 100%;
  }
}

.loaded li {
  text-transform: uppercase;
  font-size: 17px;
  text-align: left !important;
  margin-top: 17px;
  line-height: 17px;
}

.loaded li a {
  position: relative;
  color: #a5a6a6;
  -moz-transition: all .3s ease-out;
  -o-transition: all .3s ease-out;
  -webkit-transition: all .3s ease-out;
  transition: all .3s ease-out;
}

.loaded li a:hover {
  color: #1a1a1a !important;
}

.loaded li a.grow::after {
  content: "";
  height: 1px;
  width: 0;
  background-color: #3fcaab;
  position: absolute;
  bottom: -5px;
  left: 0;
  transition: width 500ms ease;
}

.loaded li a.grow:hover::after {
  width: 100%;
}

.sns {
  float: left;
  margin-top: 17px;
}

.sns li {
  margin-right: 17px;
  display: inline-block;
}

.sub_content li {
  float: left;
  width: 100%;
}

@-webkit-keyframes fadeIn {
  from {
    opacity: 0;
  }
  to {
    opacity: 1;
  }
}

@-moz-keyframes fadeIn {
  from {
    opacity: 0;
  }
  to {
    opacity: 1;
  }
}

@keyframes fadeIn {
  from {
    opacity: 0;
  }
  to {
    opacity: 1;
  }
}

.fade-in {
  opacity: 0;
  -webkit-animation: fadeIn ease-in 1;
  -moz-animation: fadeIn ease-in 1;
  animation: fadeIn ease-in 1;

  -webkit-animation-fill-mode: forwards;
  -moz-animation-fill-mode: forwards;
  animation-fill-mode: forwards;

  -webkit-animation-duration: 1s;
  -moz-animation-duration: 1s;
  animation-duration: 1s;

  -webkit-animation-delay: 1.2s;
  -moz-animation-delay: 1.2s;
  animation-delay: 1.2s;
}

.sub_content li a {
  display: block;
}

.sub_content li a img {
  width: 180px;
  height: auto;
}

.content {
  color: #ffffff;
  background-color: #3fcaab;
  font-size: 14px;
  text-align: left;
  width: 100%;
  height: 148px;
  padding: 34px 0 0 0;
  margin: 0 0 0 0 !important;
}

.content h2 {
  font-size: 14px !important;
  position: absolute !important;
  top: 0 !important;
  left: 0 !important;
  color: #ffffff !important;
}

.content .top_news {
  height: 52px;
}

.content .top_news .time {
  font-size: 10px;
  position: absolute;
  top: 0;
  float: right;
  margin-left: 67px;
}

.content a {
  font-size: 10px !important;
  text-decoration: none !important;
  color: #ffffff !important;
  position: absolute !important;
  bottom: 0 !important;
  float: right !important;
  margin-left: 67px;
}

.more_buttom {
  position: absolute;
  border: 1px solid white;
  top: -25px;
  right: 20px;
}

.more_buttom a {
  position: relative !important;
  text-align: center;
  display: block;
  font-size: 10px;
  text-decoration: none;
  color: #ffffff;
  margin: 1px 10px 1px 10px !important;
}

.content .top_twitter {
  height: 80px;
  margin-left: 5%;
}

.top_twitter .tweet_wrap {
  position: absolute;
  top: 0;
  left: 0;
  height: 80px;
}

.top_twitter p {
  display: block;
}

.top_twitter a {
  position: relative !important;
}

.lb {
  position: fixed;
  z-index: 190;
  top: 0;
  left: 0;
  bottom: 0;
  right: 0;
  width: auto;
  height: auto;
}

.lb-close {
  display: block;
  position: absolute;
  right: 1em;
  top: 1em;
  width: auto;
  height: auto;
  text-align: center;
  line-height: 0;
  padding: .5rem .5rem;
}

.lb-overlay {
  background-color: #3fcaab;
  position: fixed;
  top: 0;
  bottom: 0;
  left: 0;
  right: 0;
  z-index: 200;
  display: -webkit-box;
  display: -ms-flexbox;
  display: flex;
  -webkit-box-align: center;
  -ms-flex-align: center;
  align-items: center;
  -webkit-box-pack: center;
  -ms-flex-pack: center;
  justify-content: center;
}

.close {
  position: relative;
  display: inline-block;
  width: 35px;
  height: 35px;
  overflow: hidden;
}

.close::before,
.close::after {
  content: '';
  position: absolute;
  width: 100%;
  top: 50%;
  left: 0;
  margin-top: -1px;
  background: #fff;
}

.close::before {
  -webkit-transform: rotate(45deg);
  -moz-transform: rotate(45deg);
  -ms-transform: rotate(45deg);
  -o-transform: rotate(45deg);
  transform: rotate(45deg);
}

.close::after {
  -webkit-transform: rotate(-45deg);
  -moz-transform: rotate(-45deg);
  -ms-transform: rotate(-45deg);
  -o-transform: rotate(-45deg);
  transform: rotate(-45deg);
}

.close.hairline::before,
.close.hairline::after {
  height: 2px;
}

.batch {
  background-color: #b0e45d;
  height: 45px;
  width: 100%;
}

.sp_text {
  padding: 5px 0 5px 0;
  color: white;
  line-height: 35px;
  display: block;
  font-size: 18px;
}
</style>
