<template>
  <div class="info-wrapper">
    <div class="info-bg"></div>
    <div class="element-container info">
      <img src="@/assets/images/strategy3.webp" class="img" />
      <h6 class="title">通过BVE商业情报分析，您将</h6>
      <div class="card-list">
        <div class="left">
          <div class="card-item">
            <img src="@/assets/images/info2.png" class="item-img" />
            <p class="text">有信心加大投资，得到更高的投资回报</p>
          </div>

          <div class="card-item">
            <img src="@/assets/images/info4.png" class="item-img" />
            <p class="text">不需要花精力与时间去上网找不确定的资料，可以让你在短时间可以了解更多行内公司的发展情况</p>
          </div>

          <div class="card-item">
            <img src="@/assets/images/info6.png" class="item-img" />
            <p class="text">股票投资得到强大的信息，人脉与投资策略的支援</p>
          </div>
        </div>
        <div class="right">
          <div class="card-item">
            <img src="@/assets/images/info3.png" class="item-img" />
            <p class="text">掌握信息差，比其他人更早发现和抓住成长股</p>
          </div>
          <div class="card-item">
            <img src="@/assets/images/info5.png" class="item-img" />
            <p class="text">让你可以节省时间，在最有效率的情况下，完成对企业的过去了解，帮助你更好的判断未来</p>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup></script>

<style lang="less" scoped>
.info-wrapper {
  background-image: url('@/assets/images/info1.jpg');
  background-position: center center;
  background-size: cover;
  background-attachment: scroll;
  position: relative;
  padding: 80px 0px 60px 0px;

  .info-bg {
    background-color: #000;
    opacity: 0.5;
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
  }

  .info {
    display: flex;
    flex-direction: column;
    align-items: center;
    .img {
      width: 168px;
      height: 168px;
      z-index: 10;
    }
    .title {
      z-index: 10;
      font-size: 45px;
      color: #fff;
      margin: 30px 0;
    }

    .card-list {
      width: 100%;
      display: flex;
      justify-content: space-between;
      z-index: 10;
      .left,
      .right {
        width: 50%;
        padding: 30px;
      }
      .card-item {
        padding: 50px 20px;
        margin-bottom: 20px;
        display: flex;
        align-items: center;
        justify-content: space-between;
        background-color: #fff;
        border-radius: 10px;
        .item-img {
          width: 86px;
          height: 86px;
        }
        .text {
          color: #1a202c;
          font-size: 27px;
          font-weight: 500;
          margin-left: 25px;
          line-height: 27px;
        }
      }
    }
  }
}

// 移动端适配
@media (max-width: 600px) {
  .info-wrapper {
  background-image: url('@/assets/images/info1.jpg');
  background-position: center center;
  background-size: cover;
  background-attachment: scroll;
  position: relative;
  padding: 80px 0px 60px 0px;

  .info-bg {
    background-color: #000;
    opacity: 0.5;
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
  }

  .info {
    display: flex;
    flex-direction: column;
    align-items: center;
    .img {
      width: 90px;
      height: 90px;
      z-index: 10;
    }
    .title {
      z-index: 10;
      font-size: 30px;
      color: #fff;
      margin: 20px 0;
    }

    .card-list {
      width: 100%;
      display: flex;
      justify-content: space-between;
      z-index: 10;
      .left,
      .right {
        width: 50%;
        padding: 10px;
      }
      .card-item {
        padding: 30px 5px 30px 5px;
        margin-bottom: 20px;
        display: flex;
        flex-direction: column;
        align-items: center;
        background-color: #fff;
        border-radius: 10px;
        .item-img {
          width: 86px;
          height: 86px;
        }
        .text {
          margin-top: 10px;
          color: #1a202c;
          font-size: 18px;
          font-weight: 500;
          margin-left: 0px;
          line-height: 20px;
        }
      }
    }
  }
}
}
</style>
