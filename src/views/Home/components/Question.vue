<template>
  <div class="question-wrapper">
    <div class="element-container question">
      <h3 class="title">投资股票最常遇到的<span style="color: #004b93">6大问题</span></h3>
      <div class="split-line"></div>
      <div class="question-list">
        <div class="question-item">
          <img src="@/assets/images/question1.png" class="img" />
          <span class="text">买股票不知道该留还是该卖？</span>
        </div>

        <div class="question-item">
          <img src="@/assets/images/question2.png" class="img" />
          <span class="text">股票卖得太早，错过了大行情</span>
        </div>
        <div class="question-item">
          <img src="@/assets/images/question3.png" class="img" />
          <span class="text">不懂止损</span>
        </div>
        <div class="question-item">
          <img src="@/assets/images/question4.png" class="img" />
          <span class="text">买了好股不会涨</span>
        </div>
        <div class="question-item">
          <img src="@/assets/images/question5.png" class="img" />
          <span class="text">不懂得分辨消息带来的机会是否值得投资？</span>
        </div>
        <div class="question-item">
          <img src="@/assets/images/question6.png" class="img" />
          <span class="text">看不懂公司基本面</span>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup></script>

<style lang="less" scoped>
.question-wrapper {
  padding: 80px 0px 50px 0px;
  .question {
    display: flex;
    flex-direction: column;
    align-items: center;
    .title {
      font-size: 44px;
      font-weight: bold;
      color: #444;
      margin: 40px 0;
    }
    .split-line {
      margin: 15px 0;
      height: 4.5px;
      width: 10%;
      background-color: #004b93;
    }

    .question-list {
      display: flex;
      flex-wrap: wrap;
      padding: 60px 0 60px 60px;
      .question-item {
        padding: 50px 0px 50px 0px;
        width: 50%;
        display: flex;
        align-items: center;
        .img {
          height: 94px;
          width: 94px;
          margin-right: 30px;
        }
        .text {
          color: #1a202c;
          font-size: 27px;
          padding-right: 60px;
        }
      }
    }
  }
}

// 移动端适配
@media (max-width: 600px) {
  .question-wrapper {
    padding: 20px 0px 20px 0px;
    .question {
      display: flex;
      flex-direction: column;
      align-items: center;
      .title {
        font-size: 28px;
        font-weight: bold;
        color: #444;
        margin: 40px 0;
      }
      .split-line {
        margin: 10px 0;
        height: 4.5px;
        width: 10%;
        background-color: #004b93;
      }

      .question-list {
        display: flex;
        flex-wrap: wrap;
        padding: 20px 0 20px 20px;
        .question-item {
          padding: 20px 0px 20px 0px;
          width: 50%;
          display: flex;
          flex-direction: column;
          align-items: center;
          .img {
            height: 94px;
            width: 94px;
          }
          .text {
            color: #1a202c;
            font-size: 20px;
            margin-top: 5px;
            text-align: center;
          }
        }
      }
    }
  }
}
</style>
