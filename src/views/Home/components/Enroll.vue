<template>
  <div class="enroll-wrapper">
    <div class="element-container enroll">
      <img src="@/assets/images/enroll2.png" class="enroll-logo" />
      <h6 class="title1">BVE有行内人士为学员整合商业情报，挖掘成长股</h6>
      <div @click="playVideo = true" v-if="!playVideo" class="video-wrapper">
        <img src="@/assets/images/play-video.png" class="play-img" />
        <img src="@/assets/images/enroll3.jpg" class="enroll-img" />
      </div>
      <iframe
        v-else
        class="video-wrapper"
        src="https://www.youtube.com/embed/bY1bo7sgZ0c?controls=1&rel=0&playsinline=0&modestbranding=0&autoplay=0&enablejsapi=1&origin=https%3A%2F%2Fwww.grandpine.com&widgetid=1"
      ></iframe>
      <h6 class="title2">我想了解更多关于BVE</h6>
      <h6 class="title1">免费报名线上【投资分享会】</h6>
      <div class="button">点击报名</div>
    </div>
  </div>
</template>
<script setup>
import { ref } from 'vue'

const playVideo = ref(false)
</script>

<style lang="less" scoped>
.enroll-wrapper {
  padding: 60px 0px 90px 0px;
  background-image: url('@/assets/images/enroll1.jpg');
  background-size: cover;
  .enroll {
    display: flex;
    flex-direction: column;
    align-items: center;
    .enroll-logo {
      width: 168px;
      height: 168px;
    }
    .title1 {
      color: #fff;
      font-size: 44px;
    }

    .title2 {
      color: #fff;
      font-size: 24px;
      margin: 20px 0;
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

      .enroll-img {
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

    .button {
      margin-top: 20px;
      background-color: #008afc;
      font-size: 16px;
      color: #fff;
      padding: 12px 25px;
      border-radius: 5px;
      cursor: pointer;
      transition: all 0.6s;
      &:hover {
        transform: scale(1.1);
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
  .enroll-wrapper {
    padding: 60px 0px 90px 0px;
    background-image: url('@/assets/images/enroll1.jpg');
    background-size: cover;
    .enroll {
      display: flex;
      flex-direction: column;
      align-items: center;
      .enroll-logo {
        width: 70px;
        height: 70px;
      }
      .title1 {
        color: #fff;
        font-size: 17px;
      }

      .title2 {
        color: #fff;
        font-size: 18px;
        margin: 20px 0;
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

        .thought-img {
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

      .button {
        margin-top: 20px;
        background-color: #008afc;
        font-size: 16px;
        color: #fff;
        padding: 12px 25px;
        border-radius: 5px;
        cursor: pointer;
        transition: all 0.6s;
        &:hover {
          transform: scale(1.1);
        }
      }
    }
  }
}
</style>
