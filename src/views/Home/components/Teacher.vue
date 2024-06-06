<template>
  <div class="teacher-wrapper">
    <div class="element-container teacher">
      <h3 class="title">投资经验丰富的导师亲自授课</h3>
      <h6 class="title2">
        有经验的导师教法让您简单容易明白，就是课程内容是非常白化，新手，老人都可以容易明白，把精髓成为自己的本事。
      </h6>

      <div class="teacher-card">
        <div class="left">
          <img src="@/assets/images/teacher1.png" class="teacher-img" />
        </div>
        <div class="right">
          <div class="name">李永安老师</div>
          <div class="job">松大资本集团/中国昆辰私募基金创办人</div>
          <ul>
            <li>中国昆辰私募基金创办人，经营10亿的资金</li>
            <li>畅销书籍 “稳赚大马股市” 作者</li>
            <li>GLOBAL ENTREPRENEUR EXCHANGE（GEX）企业总监</li>
          </ul>
        </div>
      </div>
      <div class="teacher-card">
        <div class="left">
          <img src="@/assets/images/teacher2.png" class="teacher-img" />
        </div>
        <div class="right">
          <div class="name">陈剑老师</div>
          <div class="job">松大资本集团首席导师​</div>
          <ul>
            <li>拥有19 年⼤马投资教育经验的专才，教学方式生动有趣，容易理解</li>
            <li>《⼤马股市第⼀堂课》的作者，是松⼤⾥的灵魂⼈物之⼀</li>
            <li>市场一致公认的价值投资启蒙老师</li>
          </ul>
        </div>
      </div>
      <div class="teacher-card">
        <div class="left">
          <img src="@/assets/images/teacher3.jpg" class="teacher-img" />
        </div>
        <div class="right">
          <div class="name">David 老师</div>
          <div class="job">松大资本集团资产管理部总经理​</div>
          <ul>
            <li>参与基金管理及规划，也培育出超过10000个成功投资者</li>
            <li>通过16年的研究经验打造出属于松大的情报网收集来自18个行业的生意情报</li>
            <li>松⼤《最强鹰眼》，通过识别上市公司的财务报表的蛛丝马迹找到投资机会</li>
          </ul>
        </div>
      </div>
      <div class="teacher-card">
        <div class="left">
          <img src="@/assets/images/teacher4.png" class="teacher-img" />
        </div>
        <div class="right">
          <div class="name">Ms Hew老师</div>
          <div class="job">松大资本研究部总监</div>
          <ul>
            <li>女性做好投资的代表性人物</li>
            <li>提倡“生活投资法”，通过留意生活上的细节轻松找到好的投资机会</li>
            <li>有很好的统筹能⼒，在收集数据以及整理资讯的能⼒⾮常强</li>
            <li>松大《Fact find⼥王》</li>
          </ul>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup></script>

<style lang="less" scoped>
.teacher-wrapper {
  padding: 60px 0px 80px 0px;
  .teacher {
    display: flex;
    flex-direction: column;
    align-items: center;
    .title {
      font-size: 45px;
      color: #00539b;
    }
    .title2 {
      font-size: 16px;
      color: #000;
      font-weight: normal;
      margin: 30px;
    }
    .teacher-card {
      width: 100%;
      border-bottom: 4px solid #00539b;
      box-shadow: 0px 0px 10px 0px rgba(0, 0, 0, 0.5);
      margin: 10px 0;
      padding: 10px 0;
      display: flex;
      justify-content: center;
      .left {
        flex: 3;
        padding: 10px 35px;
        border-right: 1px solid #ccc;

        .teacher-img {
          width: 377px;
          height: 377px;
        }
      }
      .right {
        padding-left: 30px;
        flex: 7;
        display: flex;
        flex-direction: column;
        justify-content: center;
        .name {
          font-size: 45px;
          font-weight: bold;
        }

        .job {
          margin: 20px 0;
        }
      }
    }
  }
}

// 移动端适配
@media (max-width: 600px) {
  .teacher-wrapper {
    padding: 60px 0px 60px 0px;
    .teacher {
      display: flex;
      flex-direction: column;
      align-items: center;
      .title {
        font-size: 28px;
        color: #00539b;
      }
      .title2 {
        font-size: 14px;
        color: #000;
        font-weight: normal;
        margin: 30px 10px;
        text-align: center;
      }
      .teacher-card {
        width: 90%;
        border-bottom: 4px solid #00539b;
        box-shadow: 0px 0px 10px 0px rgba(0, 0, 0, 0.5);
        margin: 10px 0;
        padding: 10px 10px 40px 10px;
        display: flex;
        flex-direction: column;
        justify-content: center;
        .left {
          flex: 3;
          padding: 10px 15px 10px 0;
          border-right: none;

          .teacher-img {
            width: 100%;
            height: auto;
          }
        }
        .right {
          margin-top: 20px;
          padding-left: 10px;
          flex: 7;
          display: flex;
          flex-direction: column;
          justify-content: center;
          .name {
            font-size: 28px;
            font-weight: bold;
          }

          .job {
            margin: 20px 0;
            font-size: 15px;
          }

          ul {
            padding-left: 30px;
            font-size: 15px;
          }
        }
      }
    }
  }
}
</style>
