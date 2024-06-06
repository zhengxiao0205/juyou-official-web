<template>
  <div class="case1-wrapper">
    <div class="element-container case1">
      <div class="data-card">
        <div class="top">
          <div class="data-item">
            <p class="number">8</p>
            <span class="text">位资深导师</span>
          </div>
          <div class="data-item">
            <p class="number">18</p>
            <span class="text">行业</span>
          </div>
          <div class="data-item">
            <p class="number">23</p>
            <span class="text">子行业</span>
          </div>
        </div>
        <div class="bottom">
          <div>为你周日每天持续不断报道和整合可靠商业情报，集合不同生意的行内信息,</div>
          <div>通过视频为你分析公司内在价值,发展，风险，找出成长股</div>
        </div>
      </div>

      <div class="case">
        <h6 class="title">案例分享 :</h6>
        <img src="@/assets/images/case1.png" class="img" />

        <div class="card-list">
          <div class="card-item">
            <div class="card-top">
              <h6 class="year">2018</h6>
              <div class="label">管理层实时更新</div>
              <ul>
                <li>第一次参观D&O工厂 专访CEO</li>
              </ul>
              <div class="label">松大信息网</div>
              <ul>
                <li>R&D 部门正在研发新的汽车LED产品</li>
                <li>D&O 与 BMW 合作开发 Smart RGB LED</li>
              </ul>
            </div>
            <img src="@/assets/images/case2.jpg" class="card-img" />
          </div>

          <div class="card-item">
            <div class="card-top">
              <h6 class="year">2019</h6>
              <div class="label">管理层实时更新</div>
              <ul>
                <li>第二次拜访D&O 了解新工厂建造当中</li>
              </ul>
              <div class="label">松大信息网</div>
              <ul>
                <li>升级至双层生产线，用于增加产能</li>
                <li>成立新部门，为客户提供模块化组装作为增值服务</li>
              </ul>
            </div>
            <img src="@/assets/images/case3.jpg" class="card-img" />
          </div>
          <div class="card-item">
            <div class="card-top">
              <h6 class="year">2020</h6>
              <div class="label">管理层实时更新</div>
              <ul>
                <li>新工厂正式启用 了解新工厂建造当中</li>
              </ul>
              <div class="label">松大信息网</div>
              <ul>
                <li>总部及办公室搬迁至新楼，旧楼空间腾出用于生产线</li>
                <li>原料短缺问题对生产线影响不大</li>
              </ul>
            </div>
            <img src="@/assets/images/case4.jpg" class="card-img" />
          </div>
          <div class="card-item">
            <div class="card-top">
              <h6 class="year">2021</h6>
              <div class="label">管理层实时更新</div>
              <ul>
                <li>新联营公司“Domi-Star”继续开发新产品</li>
              </ul>
              <div class="label">松大信息网</div>
              <ul>
                <li>生产线一直非常繁忙，因为整个 2021 年的订单都已满负荷运转</li>
                <li>电动汽车的高需求增加了LED的需求，尤其是中国市场</li>
              </ul>
            </div>
            <img src="@/assets/images/case5.jpg" class="card-img" />
          </div>
        </div>

        <img src="@/assets/images/case6.png" class="chart-img" />
      </div>
    </div>
  </div>
</template>

<script setup></script>

<style lang="less" scoped>
.case1-wrapper {
  padding: 30px 0px 90px 0px;
  background-color: #fff;
  .case1 {
    display: flex;
    flex-direction: column;
    align-items: center;
    .data-card {
      width: 98%;
      z-index: 10;
      background-color: #fff;
      border-bottom: 4px solid #d3b574;
      box-shadow: 0px 0px 30px 0px rgba(0, 0, 0, 0.15);
      margin-top: -90px;
      padding: 30px 20px 45px 20px;
      display: flex;
      flex-direction: column;
      align-items: center;
      .top {
        width: 90%;
        display: flex;
        justify-content: center;
        align-items: center;
        .data-item {
          display: flex;
          flex-direction: column;
          align-items: center;
          flex: 1;
          border-right: 1px solid #aaa;
          &:last-child {
            border-right: none;
          }
          .number {
            font-size: 60px;
            color: #000;
            font-weight: bold;
            margin: 5px 0;
          }
          .text {
            font-size: 16px;
            color: #4a4a4a;
          }
        }
      }

      .bottom {
        margin-top: 50px;
        width: 80%;
        font-size: 20px;
        font-weight: bold;
        text-align: center;
      }
    }

    .case {
      margin-top: 50px;
      display: flex;
      flex-direction: column;
      align-items: center;
      .title {
        font-size: 32px;
        color: #000;
      }

      .img {
        margin-top: 20px;
        width: 330px;
      }

      .card-list {
        margin-top: 20px;
        display: flex;
        justify-content: space-between;
        .card-item {
          box-shadow: 0px 0px 20px 0px rgba(0, 0, 0, 0.15);
          margin: 0 10px;
          border-top: 4px solid #6c6b7d;
          display: flex;
          flex-direction: column;
          justify-content: space-between;
          .card-top {
            padding: 35px;
            .year {
              font-size: 20px;
              font-weight: 600;
            }
            .label {
              margin-top: 15px;
              color: #4a4a4a;
              font-weight: bold;
            }
            ul {
              margin-top: 4px;
              padding-left: 15px;
              li {
                color: #4a4a4a;
                font-size: 14px;
                font-weight: 100;
                margin-top: 3px;
              }
            }
          }
          .card-img {
            width: 100%;
          }
        }
      }

      .chart-img {
        width: 98%;
        object-fit: cover;
        margin-top: 25px;
        border: 3px solid #000;
        border-radius: 15px;
      }
    }
  }
}

// 移动端适配
@media (max-width: 600px) {
  .case1-wrapper {
    padding: 30px 0px 30px 0px;
    background-color: #fff;
    .case1 {
      display: flex;
      flex-direction: column;
      align-items: center;
      .data-card {
        width: 85%;
        z-index: 10;
        background-color: #fff;
        border-bottom: 4px solid #d3b574;
        box-shadow: 0px 0px 30px 0px rgba(0, 0, 0, 0.15);
        margin-top: -90px;
        padding: 30px 20px 45px 20px;
        display: flex;
        flex-direction: column;
        align-items: center;
        .top {
          width: 90%;
          display: flex;
          justify-content: center;
          align-items: center;
          .data-item {
            display: flex;
            flex-direction: column;
            align-items: center;
            flex: 1;
            border-right: none;

            .number {
              font-size: 28px;
              color: #000;
              font-weight: bold;
              margin: 5px 0;
            }
            .text {
              font-size: 14px;
              color: #4a4a4a;
            }
          }
        }

        .bottom {
          margin-top: 50px;
          width: 90%;
          font-size: 14px;
          font-weight: bold;
          text-align: center;
        }
      }

      .case {
        margin-top: 50px;
        display: flex;
        flex-direction: column;
        align-items: center;
        .title {
          font-size: 30px;
          color: #000;
        }

        .img {
          margin-top: 20px;
          width: 234px;
        }

        .card-list {
          margin-top: 20px;
          display: flex;
          flex-direction: column;
          align-items: center;
          .card-item {
            box-shadow: 0px 0px 20px 0px rgba(0, 0, 0, 0.15);
            margin: 0 10px;
            border-top: 4px solid #6c6b7d;
            display: flex;
            flex-direction: column;
            justify-content: space-between;
            .card-top {
              padding: 35px;
              .year {
                font-size: 20px;
                font-weight: 600;
              }
              .label {
                margin-top: 15px;
                color: #4a4a4a;
                font-weight: bold;
              }
              ul {
                margin-top: 4px;
                padding-left: 15px;
                li {
                  color: #4a4a4a;
                  font-size: 14px;
                  font-weight: 100;
                  margin-top: 3px;
                }
              }
            }
            .card-img {
              width: 100%;
            }
          }
        }

        .chart-img {
          display: none;
        }
      }
    }
  }
}
</style>
