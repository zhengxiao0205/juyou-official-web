<template>
  <div class="investor-wrapper">
    <img src="@/assets/images/investor.jpg" class="img" />

    <div class="element-container investor">
      <h3 class="title">超过20,000名投资散户已参加BIS</h3>
      <div class="button">松大学员们的成功案例</div>
    </div>
  </div>
</template>

<script setup></script>

<style lang="less" scoped>
.investor-wrapper {
  overflow: hidden;
  position: relative;
  height: 280px;

  .img {
    width: 100%;
    height: 100%;
    object-fit: cover;
    transition: all 2s;
    position: absolute;
  }
  .investor {
    height: 100%;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;

    .title {
      font-size: 40px;
      color: #fff;
      margin-bottom: 20px;
      z-index: 10;
      transition: all 1s;
    }
    .button {
      cursor: pointer;
      color: #fff;
      background-color: transparent;
      font-size: 16px;
      padding: 10px 20px;
      border-radius: 5px;
      border: 1px solid #fff;
      z-index: 10;
      transition: all 1s;
    }
  }

  &:hover {
    .img {
      transform: scale(1.2); // 图片放大
    }

    .title {
      transform: scale(1.1); // 文字放大
    }

    .button {
      transform: scale(1.1); // 按钮放大
    }
  }
}

// 移动端适配
@media (max-width: 600px) {
  .title {
    font-size: 24px !important;
    text-align: center;
  }
}
</style>
