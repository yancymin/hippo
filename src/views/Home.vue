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
        <li class="icon">
          <a>
            <div class="img-wrap">
              <img src="../assets/wechat.svg" alt>
            </div>WeChat
          </a>
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

<style lang="scss" scoped>
.home {
  width: 100vw;
  height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;

  .container {
    position: relative;
    width: 700px;
    height: 400px;
    background: url("../assets/screen-bg.jpg");
    background-size: cover;
    overflow: hidden;

    .icon-wrap {
      position: absolute;
      left: 215px;
      top: 30px;
      width: 224px;
      height: 210px;
      display: flex;
      justify-content: space-between;
      align-content: space-between;
      flex-wrap: wrap;
      li {
        position: relative;
        width: 64px;
        height: 64px;
        display: flex;
        justify-content: center;
        align-items: center;

        &:nth-of-type(3) {
          visibility: hidden;
          opacity: 0;
        }
        &:nth-of-type(9) {
          visibility: hidden;
          opacity: 0;
        }

        a {
          display: flex;
          justify-content: center;
          flex-direction: column;
          width: 100%;
          height: 100%;
          font-size: 12px;
          font-weight: 600;
          color: #ffffff;
          letter-spacing: 0;
          text-shadow: 0 0 1px rgba(0, 0, 0, 0.5);
          text-decoration-line: none;
          white-space: nowrap;
          margin-top: 16px;
          transform: scale(0.9);
          cursor: pointer;

          &::before {
            z-index: -1;
            opacity: 0;
            content: "";
            position: absolute;
            left: -8px;
            display: block;
            width: 100%;
            height: 100%;
            background-color: #e1b9a7;
            padding: 8px;
            border-radius: 6px;
            transition: all 0.2s ease-out;
          }

          &:hover::before {
            opacity: 1;
          }

          .img-wrap {
            width: 100%;
            height: 100%;
            display: flex;
            justify-content: center;
            align-items: center;
          }

          img {
            margin-bottom: 6px;
          }
        }
      }
    }

    .dialog {
      z-index: 999;
      opacity: 1;

      .dialog-wrap {
        li {
          opacity: 0;
          display: flex;
          justify-content: flex-start;
          align-items: center;
          position: absolute;
          padding: 8px 14px;
          background-color: #464646;
          border-radius: 6px;
          color: #fff;
          font-size: 12px;
          text-align: left;
          right: 0;
          margin-right: 20px;
          animation: dialogShow 0.6s ease-in-out forwards;

          p {
            transform: scale(0.9);
          }

          img {
            width: 32px;
            height: 32px;
          }

          strong {
            font-weight: 800;
          }

          &::before {
            content: "";
            display: block;
            position: absolute;
            right: -5px;
            bottom: 10px;
            width: 10px;
            height: 10px;
            border-radius: 1px;
            background-color: #464646;
            transform: rotate(45deg);
          }

          &:nth-of-type(1) {
            top: 20px;
            animation-delay: 1.2s;
              transform: translateX(100px);
          }
          &:nth-of-type(2) {
            top: 75px;
            animation-delay: 1.8s;
              transform: translateX(100px);
          }
          &:nth-of-type(3) {
            top: 130px;
            animation-delay: 2.4s;
              transform: translateX(100px);
          }

          @keyframes dialogShow {
           to {
             transform: translateX(0);
             opacity: 1;
           }
          }
        }
      }
    }
  }
}
</style>
