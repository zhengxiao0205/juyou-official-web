<template>
  <div class="question2-wrapper">
    <div class="element-container question2">
      <h3 class="title1">上面这六个问题是我们经过20年的投资教学经验所收到的普遍投资者常碰到的问题</h3>
      <h3 class="title2">有哪一个 / 几个是你面对到的吗？</h3>
    </div>
  </div>
</template>

<script setup></script>

<style lang="less" scoped>
.question2-wrapper {
  padding: 80px 0px 80px 0px;
  background-color: #727272;
  opacity: 0.89;
  .question2 {
    min-height: 400px;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    .title1 {
      font-size: 28px;
      color: #fff;
      margin-bottom: 40px;
      text-align: center;
    }
    .title2 {
      font-size: 40px;
      color: #fff;
    }
  }
}

// 移动端适配
@media (max-width: 600px) {
  .question2-wrapper {
    padding: 40px 20px 40px 20px;
    background-color: #727272;
    opacity: 0.89;
    .question2 {
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      .title1 {
        font-size: 24px;
        color: #fff;
        margin-bottom: 40px;
        text-align: center;
      }
      .title2 {
        font-size: 36px;
        color: #fff;
        text-align: center;
      }
    }
  }
}
</style>
