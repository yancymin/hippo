<template>
  <div class="home">
    <div class="container">
      <ul class="icon-wrap">
        <li class="icon">
          <a href="http://hwoma.lofter.com/post/2006399c_12df62af6 " target="_blank">
            <div class="img-wrap">
              <img src="../assets/design-work.svg" alt>
            </div>Work
          </a>
        </li>
        <li class="icon">
          <a href="https://www.zcool.com.cn/u/17018264" target="_blank">
            <div class="img-wrap">
              <img src="../assets/zcool.svg" alt>
            </div>站酷
          </a>
        </li>
        <li class="icon">
          <a href>/</a>
        </li>
        <li class="icon">
          <a href="https://www.weibo.com/3175887084" target="_blank">
            <div class="img-wrap">
              <img src="../assets/weibo1.svg" alt>
            </div>Weibo
          </a>
        </li>
        <li class="icon">
          <a href="https://dribbble.com/Bhippo" target="_blank">
            <div class="img-wrap">
              <img src="../assets/dribbble.svg" alt>
            </div>Dribbble
          </a>
        </li>
        <li class="icon">
          <a href="https://www.instagram.com/huoma_bao/" target="_blank">
            <div class="img-wrap">
              <img src="../assets/ig.svg" alt>
            </div>Instagram
          </a>
        </li>
        <li class="icon">
          <a href="mailto:947588644@qq.com" target="_blank">
            <div class="img-wrap">
              <img src="../assets/Email.svg" alt>
            </div>Email me
          </a>
        </li>
        <li class="icon" id="wechat">
          <a>
            <div class="img-wrap">
              <img src="../assets/wechat.svg" alt>
            </div>WeChat
          </a>
          <i id="qr" class="qr"></i>
        </li>
        <li class="icon">
          <a href></a>
        </li>
      </ul>
      <div class="dialog">
        <ul class="dialog-wrap">
          <li>
            <img src="../assets/me.png" alt>
            <p>Hi，You found me！</p>
          </li>
          <li>
            <img src="../assets/me.png" alt>
            <p>
              I’m
              <strong>Hwoma～</strong> Nice to meet you！
            </p>
          </li>
          <li>
            <img src="../assets/me.png" alt>
            <p>
              I’m a
              <strong>designer</strong>.
              <br>Based in
              <strong>Wuhan, China</strong>
            </p>
          </li>
        </ul>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  mounted: function() {
    var wechat = document.getElementById("wechat");
    var qr = document.getElementById("qr");

    wechat.addEventListener("mouseenter", function() {
      qr.classList.add("qrShow");

      if (
        wechat.addEventListener("mouseleave", function() {
          qr.classList.remove("qrShow");
        })
      ) {
      }
    });
  }
};
</script>

<style lang="scss" scoped>
@import "../style/main.scss";
</style>

