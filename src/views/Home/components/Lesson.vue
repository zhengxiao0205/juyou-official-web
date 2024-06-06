<template>
  <div class="lesson-wrapper">
    <div class="element-container lesson">
      <img src="@/assets/images/lesson1.png" class="lesson-logo" />
      <h6 class="lesson-title">20天完整线上价值投资课程</h6>
      <img src="@/assets/images/lesson2.png" class="lesson-logo2" />
      <h6 class="lesson-title2">-受大马人力资源发展机构认证-</h6>
      <div @click="playVideo = true" v-if="!playVideo" class="video-wrapper">
        <img src="@/assets/images/play-video.png" class="play-img" />
        <img src="@/assets/images/lesson3.jpg" class="lesson-img" />
      </div>
      <iframe
        v-else
        class="video-wrapper"
        src="https://www.youtube.com/embed/IVorlAPBD3c?controls=1&rel=0&playsinline=0&modestbranding=0&autoplay=0&enablejsapi=1&origin=https%3A%2F%2Fwww.grandpine.com&widgetid=1"
      ></iframe>
      <div class="text-wrapper">
        <span class="text">掌握完整价值投资策略</span>
      </div>
      <div class="lesson-list">
        <div class="lesson-item">
          <img src="@/assets/images/lesson4.png" class="item-img" />
          <div class="split-line"></div>
          <div class="item-text">
            <div>预录和直播讲解</div>
            <div>(一年内无限次复习)</div>
          </div>
        </div>
        <div class="lesson-item">
          <img src="@/assets/images/lesson5.png" class="item-img" />
          <div class="split-line"></div>
          <div class="item-text">
            <div>每个小单元都有一个功课加上Q&A环节</div>
          </div>
        </div>
        <div class="lesson-item">
          <img src="@/assets/images/lesson6.png" class="item-img" />
          <div class="split-line"></div>
          <div class="item-text">
            <div>势必让你掌握每个细节，用生意的思维帮助我们了解企业的内在价值和发展前景</div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
import { ref } from 'vue'

const playVideo = ref(false)
</script>

<style lang="less" scoped>
.lesson-wrapper {
  padding: 30px 0px 60px 0px;
  background-color: #f8f9fa;
  border-bottom: 1px solid #d6d6d6;
  .lesson {
    display: flex;
    flex-direction: column;
    align-items: center;
    .lesson-logo {
      width: 30%;
    }
    .lesson-title {
      color: #004185;
      font-size: 44px;
    }
    .lesson-logo2 {
      margin-top: 10px;
      width: 269px;
      height: 150px;
    }
    .lesson-title2 {
      color: #57586e;
      font-size: 24px;
    }
    .video-wrapper {
      margin-top: 15px;
      border-radius: 10px;
      width: 1120px;
      height: 630px;
      display: flex;
      justify-content: center;
      align-items: center;
      position: relative;
      cursor: pointer;

      .lesson-img {
        position: absolute;
        width: 100%;
        height: 100%;
      }

      .play-img {
        z-index: 10;
        width: 100px;
        height: 100px;
      }
    }

    .text-wrapper {
      margin-top: 30px;
      width: 98%;
      color: #00539b;
      font-size: 32px;
      display: flex; // 左横线，文字，右横线flex布局
      align-items: center;
      font-weight: 100;
      .text {
        padding: 0 10px; // 文字和左右横线的间距
      }

      // 前后的横线用before和after伪类呈现
      &::before,
      &::after {
        flex: 1;
        content: '';
        height: 1px;
        background-color: #00539b;
      }
    }

    .lesson-list {
      margin-top: 100px;
      display: flex;
      justify-content: center;
      width: 90%;
      .lesson-item {
        display: flex;
        flex-direction: column;
        align-items: center;
        flex: 1;
        .item-img {
          width: 155px;
          height: 155px;
        }

        .split-line {
          background-color: #00539b;
          height: 5px;
          width: 20%;
          margin: 40px 0;
        }
        .item-text {
          text-align: center;
          width: 85%;
          color: #444;
        }
      }
    }
  }
}

@media (max-width: 1200px) {
  .video-wrapper {
    width: 960px !important;
    height: 540px !important;
  }
}
// 移动端适配
@media (max-width: 600px) {
  .lesson-wrapper {
    padding: 30px 0px 60px 0px;
    background-color: #F8F9FA;
    border-bottom: 1px solid #d6d6d6;
    .lesson {
      display: flex;
      flex-direction: column;
      align-items: center;
      .lesson-logo {
        width: 30%;
      }
      .lesson-title {
        color: #004185;
        font-size: 28px;
      }
      .lesson-logo2 {
        margin-top: 10px;
        width: 269px;
        height: 150px;
      }
      .lesson-title2 {
        color: #57586e;
        font-size: 16px;
      }
      .video-wrapper {
        margin-top: 15px;
        border-radius: 10px;
        width: 95% !important;
        height: 225px !important;
        display: flex;
        justify-content: center;
        align-items: center;
        position: relative;
        cursor: pointer;

        .lesson-img {
          position: absolute;
          width: 100%;
          height: 100%;
        }

        .play-img {
          z-index: 10;
          width: 80px;
          height: 80px;
        }
      }

      .text-wrapper {
        margin-top: 30px;
        width: 95%;
        color: #00539b;
        font-size: 26px;
        display: flex; // 左横线，文字，右横线flex布局
        align-items: center;
        font-weight: 100;
        .text {
          padding: 0 10px; // 文字和左右横线的间距
        }

        // 前后的横线用before和after伪类呈现
        &::before,
        &::after {
          flex: 1;
          content: '';
          height: 1px;
          background-color: #00539b;
        }
      }

      .lesson-list {
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        width: 90%;
        .lesson-item {
          display: flex;
          flex-direction: column;
          align-items: center;
          margin-bottom: 80px;
          &:last-child {
            margin-bottom: 0px;
          }
          .item-img {
            width: 190px;
            height: 190px;
          }

          .split-line {
            background-color: #00539b;
            height: 5px;
            width: 80px;
            margin: 40px 0;
          }
          .item-text {
            text-align: center;
            width: 85%;
            color: #444;
          }
        }
      }
    }
  }
}
</style>
