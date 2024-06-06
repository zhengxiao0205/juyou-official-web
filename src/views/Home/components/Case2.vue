<template>
  <div class="case2-wrapper">
    <div class="element-container case2">
      <div class="case">
        <h6 class="title">案例分享 :</h6>
        <img src="@/assets/images/case7.png" class="img" />

        <div class="card-list">
          <div class="card-item">
            <div class="card-top">
              <h6 class="year">2018</h6>
              <div class="label">管理层实时更新</div>
              <ul>
                <li>参考过去2015-2017业绩，盈利增长了超过100%</li>
                <li>从CCM母公司的重组架构以后，正式成立CCM Duopharma,专门研发仿制药的生产商</li>
                <li>继续与PanGen韩国公司研发生物仿制药</li>
              </ul>
              <div class="label">松大信息网</div>
              <ul>
                <li>从药制行业学员 Fact Find 得知 CCM Duopharma 获得胰岛素供应代理权予大马卫生局，为期3年合约</li>
              </ul>
            </div>
            <img src="@/assets/images/case8.jpg" class="card-img" />
          </div>

          <div class="card-item">
            <div class="card-top">
              <h6 class="year">2019</h6>
              <div class="label">管理层实时更新</div>
              <ul>
                <li>参观Duopharma 位于 Bangi 的制药工厂并详细理解制药过程与运作</li>
                <li>亲自拜访CEO及访谈关于公司未来发展趋势</li>
              </ul>
              <div class="label">松大信息网</div>
              <ul>
                <li>升级至双层生产线，用于增加产能</li>
              </ul>
            </div>
            <img src="@/assets/images/case9.jpg" class="card-img" />
          </div>
          <div class="card-item">
            <div class="card-top">
              <h6 class="year">2020</h6>
              <div class="label">管理层实时更新</div>
              <ul>
                <li>参加股东大会以跟进最新的发展动向</li>
              </ul>
              <div class="label">松大信息网</div>
              <ul>
                <li>于医疗行业的专业人士探讨DPHARMA的疫苗瓶装生意潜能</li>
              </ul>
            </div>
            <img src="@/assets/images/case10.jpeg" class="card-img" />
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
            <img src="@/assets/images/case11.jpg" class="card-img" />
          </div>
        </div>

        <img src="@/assets/images/case12.png" class="chart-img" />
      </div>
    </div>
  </div>
</template>

<script setup></script>

<style lang="less" scoped>
.case2-wrapper {
  padding: 30px 0px 90px 0px;
  background-color: #f4f4f4;
  .case2 {
    display: flex;
    flex-direction: column;
    align-items: center;

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
            width: 265px;
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
  .case2-wrapper {
    padding: 30px 0px 30px 0px;
    background-color: #f4f4f4;
    .case2 {
      display: flex;
      flex-direction: column;
      align-items: center;

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
