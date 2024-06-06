<template>
  <div class="strategy-wrapper">
    <div class="strategy-bg"></div>
    <div class="element-container strategy">
      <div class="top">
        <div class="left">
          <img src="@/assets/images/strategy2.png" class="left-img" />
        </div>
        <div class="split-line"></div>
        <div class="right">
          <img src="@/assets/images/strategy3.webp" class="right-img" />
        </div>
      </div>
      <div class="bottom">Business Investment Strategy 还包含了Business Value Exchange (BVE) 商业情报交流平台</div>
    </div>
  </div>
</template>

<script setup></script>

<style lang="less" scoped>
.strategy-wrapper {
  background-image: url('@/assets/images/strategy1.jpg');
  background-position: center center;
  background-size: cover;
  background-attachment: fixed;
  padding: 80px 0px 80px 0px;
  position: relative;

  .strategy-bg {
    background-color: #000;
    opacity: 0.65;
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
  }

  .strategy {
    display: flex;
    flex-direction: column;
    align-items: center;
    height: 400px;

    .top {
      display: flex;
      justify-content: center;
      align-items: center;
      z-index: 10;

      .left,
      .right {
        width: 50%;
        padding: 20px;
        .left-img {
          width: 80%;
          float: right;
        }
        .right-img {
          width: 216px;
          height: 216px;
        }
      }
      .split-line {
        height: 100%;
        width: 2px;
        background-color: #fff;
      }
    }

    .bottom {
      color: #fff;
      font-size: 20px;
      margin-top: 30px;
      font-weight: bold;
      z-index: 10;
    }
  }
}

// 移动端适配
@media (max-width: 600px) {
  .strategy-wrapper {
    background-image: url('@/assets/images/strategy1.jpg');
    background-position: center 100%;
    background-size: cover;
    background-attachment: scroll;
    padding: 80px 0px 80px 0px;
    position: relative;

    .strategy-bg {
      background-color: #000;
      opacity: 0.65;
      position: absolute;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
    }

    .strategy {
      display: flex;
      flex-direction: column;
      align-items: center;
      height: 400px;

      .top {
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        z-index: 10;

        .left,
        .right {
          width: 100%;
          padding: 0px;
          display: flex;
          justify-content: center;
          align-items: center;
          .left-img {
            width: 330px;
            height: 136px;
          }
          .right-img {
            width: 132px;
            height: 132px;
          }
        }
        .split-line {
          display: none;
          height: 100%;
          width: 2px;
          background-color: #fff;
        }
      }

      .bottom {
        color: #fff;
        font-size: 16px;
        margin-top: 30px;
        font-weight: bold;
        z-index: 10;
        text-align: center;
        padding: 0 20px;
      }
    }
  }
}
</style>
