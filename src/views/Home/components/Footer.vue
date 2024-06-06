<template>
  <div class="footer-wrapper">
    <div class="element-container footer">
      <div class="disclaimer">
        <div @click="handleExpand" class="collapse-header">
          <span class="title">Disclaimer</span>
          <img v-if="!expand" class="right-img" src="@/assets/images/footer1.png" />
          <img v-else class="right-img" src="@/assets/images/footer2.png" />
        </div>
        <div class="content" :style="{ height: expand ? 'auto' : 0 }">
          <p>
            The information and materials contained in Grandpine Capital Sdn. Bhd.'s services platforms and training
            programmes are provided to you for the purpose of general market commentary and general
            information/circulation only and is not intended to nor will it create/induce the creation of any binding
            legal relations. Our goal is to help you take control of your financial well-being by delivering solid
            investment financial education. Any opinions, news, research, analysis, prices or other information
            contained herein or obtained through our services platforms or training programmes do not constitute
            investment advice, a recommendation, a solicitation or an offer to subscribe for, purchase, sell or dispose
            of any investment or securities of any type, or to engage in any financial transaction. It does not take
            into account of your specific investment objectives, financial situation and any of your particular needs.
            Please do not trade or invest based solely on the information or materials provided by GrandPine Capital
            Sdn. Bhd.
          </p>
          <p>
            The information or materials provided should not be used without first assessing the suitability of the
            investment products, your specific investment objectives, financial situation or particular needs, or
            without seeking for the advices of qualified and competent investment professionals. By viewing the
            information within our services platform(s) and registering for our training programmes, you agree that no
            warranty whatsoever is given and no liability whatsoever is accepted for any loss or damages arising whether
            directly or indirectly as a result of any person or group of persons relying on any information obtained
            through the services platform(s) or training programmes offered by GrandPine Capital Sdn. Bhd., its
            employees, speakers, directors or fellow members. If you choose to ignore our disclaimer and do not do
            independent research of the various industries, companies, and stocks you intend to invest in and rely
            solely on the information, materials and opinions obtained through our services platforms or training
            programmes - you agree that you have made a conscious, personal decision of your own free will and will not
            try to hold us responsible for the results thereof under any circumstance.
          </p>
          <p>
            We believe we have great community of investors looking to achieve and help each other achieve financial
            success through investing. Accordingly, we encourage our community to exchange personal investment
            information during the training programmes, however, there will be times when people provide misleading,
            deceptive or incorrect information, unintentionally or otherwise. It is your responsibility to invest wisely
            and to safeguard your personal and financial information.
          </p>
          <p>
            Services platforms and training programmes of GrandPine Capital Sdn. Bhd. are offered to help you understand
            how to make good investment and personal financial decisions for yourself. You are solely responsible for
            the investment decisions you make. Our services offered herein are not for the purpose of acting as your
            personal investment advisor. We do not know all the relevant facts about you and/or your individual needs,
            and we do not represent or claim that any of our services are suitable for your needs. You should seek a
            registered investment advisor if you are looking for personalised advice.
          </p>
          <p>
            By purchasing and using any services provided by GrandPine Capital Sdn. Bhd., you expressly agree that all
            risks of the use of our services and any consequences of such use shall be borne exclusively by you. Nothing
            on this page, our website, our services platforms, our training programmes, or any other service provided by
            GrandPine Capital Sdn. Bhd. is a promise or guarantee of any results, including that you will make any
            particular amount of money, or any money at all. You also understand that all investments come with some
            risks and you may actually experience financial loss while investing. Any results stated in our services
            platforms or during our training programmes, in the form of testimonials, case studies or otherwise are
            solely for the purpose of concepts illustration and should not be taken and considered as average results,
            or promises for actual or future performance.
          </p>
          <p>
            While every effort is made to check the accuracy of the information and materials provided on our services
            platforms and training programmes, GrandPine Capital Sdn. Bhd. cannot accept responsibility for any errors
            or omissions. We therefore strongly recommend that our investor community make their own thorough checks and
            seek independent investment advice before entering into any kind of transaction.
          </p>
        </div>
      </div>
      <div class="footer-info">
        <div class="col1">
          <img class="logo-img" src="@/assets/images/footer3.png" />
          <p>GrandPine Capital Sdn Bhd (623304-K)</p>
          <p>40-3 & 42-3, Jalan PJU 8/5b, Damansara Perdana, 47820 Petaling Jaya, Selangor</p>
          <p>info@grandpine.com</p>
          <p>03-7727 0671</p>
          <div class="link-buttons">
            <div class="btn">
              <img class="btn-img" src="@/assets/images/footer4.png" />
            </div>
            <div class="btn">
              <img class="btn-img" src="@/assets/images/footer5.png" />
            </div>
            <div class="btn">
              <img class="btn-img" src="@/assets/images/footer6.png" />
            </div>
          </div>
        </div>
        <div class="col2">
          <div class="label">Courses</div>
          <div class="item">
            <p>Business Investment Strategy</p>
            <p>季度业绩投资策略</p>
          </div>
        </div>
        <div class="col3">
          <div class="label">Software</div>
          <div class="item">
            <p>Algobox</p>
            <p>ValueFarm</p>
          </div>
        </div>
        <div class="col4">
          <div class="label">Blogs</div>
          <div class="label">Shop</div>
          <div class="label">About Us</div>
          <div class="label">Contact Us</div>
          <div class="label">Disclaimer</div>
          <div class="label">Privacy Policy</div>
        </div>
      </div>
    </div>
    <div class="split-line"></div>
    <p class="element-container copyright">© 2024 Grandpine Capital Sdn Bhd. All rights reserved</p>
  </div>
</template>

<script setup>
import { ref } from 'vue'

const expand = ref(false)

const handleExpand = () => {
  expand.value = !expand.value
}
</script>

<style lang="less" scoped>
.footer-wrapper {
  padding: 60px 0px 0px 0px;
  background-color: #001c38;
  .footer {
    display: flex;
    flex-direction: column;
    align-items: center;
    .disclaimer {
      width: 98%;
      border-bottom: 1px solid #fff;
      .collapse-header {
        padding: 0px 20px;
        display: flex;
        justify-content: space-between;
        cursor: pointer;
        .title {
          color: #fff;
          font-weight: bold;
        }

        .right-img {
          width: 16px;
          height: 16px;
        }
      }
      .content {
        font-size: 13px;
        color: #dbdbdb;
        padding: 10px 20px;
        height: 100%;
        overflow: hidden;
        p {
          margin: 10px 0;
        }
      }
    }

    .footer-info {
      width: 98%;
      padding: 60px 20px;
      display: flex;
      justify-content: space-between;
      .col1 {
        width: 35%;
        .logo-img {
          width: 356px;
          height: 91px;
        }
        p {
          color: rgba(255, 255, 255, 0.65);
          font-size: 13px;
          margin: 10px 0;
        }
        .link-buttons {
          margin-top: 30px;
          display: flex;
          .btn {
            background-color: #364c62;
            border-radius: 5px;
            padding: 5px 10px;
            cursor: pointer;
            margin-right: 10px;
            .btn-img {
              width: 16px;
              height: 16px;
              position: relative;
              top: 1px;
            }
          }
        }
      }
      .col2 {
        width: 20%;
        .label {
          color: #fff;
          font-size: 18px;
        }
        .item {
          margin-top: 20px;
          color: rgba(255, 255, 255, 0.6);
          font-size: 14px;
        }
      }
      .col3 {
        width: 15%;
        .label {
          color: #fff;
          font-size: 18px;
        }
        .item {
          margin-top: 20px;
          color: rgba(255, 255, 255, 0.6);
          font-size: 14px;
        }
      }
      .col4 {
        width: 20%;
        .label {
          color: #fff;
          font-size: 18px;
          margin-bottom: 20px;
        }
      }
    }
  }

  .split-line {
    width: 100%;
    height: 1px;
    background-color: rgba(255, 255, 255, 0.6);
  }

  .copyright {
    padding: 15px 0;
    color: #adadad;
    font-size: 12px;
  }
}

@media (max-width: 1200px) {
  .logo-img {
    width: 316px !important;
    height: 81px !important;
  }
}

// 移动端适配
@media (max-width: 600px) {
  .footer-wrapper {
    padding: 60px 0px 0px 0px;
    background-color: #001c38;
    .footer {
      display: flex;
      flex-direction: column;
      align-items: center;
      .disclaimer {
        width: 98%;
        border-bottom: 1px solid #fff;
        .collapse-header {
          padding: 0px 20px;
          display: flex;
          justify-content: space-between;
          cursor: pointer;
          .title {
            color: #fff;
            font-weight: bold;
          }

          .right-img {
            width: 16px;
            height: 16px;
          }
        }
        .content {
          font-size: 13px;
          color: #dbdbdb;
          padding: 10px 20px;
          height: 100%;
          overflow: hidden;
          p {
            margin: 10px 0;
          }
        }
      }

      .footer-info {
        padding: 60px 0px;
        display: flex;
        flex-wrap: wrap;
        justify-content: space-between;
        .col1 {
          width: 100%;
          display: flex;
          flex-direction: column;
          margin-bottom: 30px;
          .logo-img {
            width: 90% !important;
            height: auto !important;
          }
          p {
            color: rgba(255, 255, 255, 0.65);
            font-size: 14px;
            margin: 10px 0;
            padding-left: 20px;
          }
          .link-buttons {
            margin-top: 30px;
            display: flex;
            padding-left: 20px;
            .btn {
              background-color: #364c62;
              border-radius: 5px;
              padding: 4px 8px;
              cursor: pointer;
              margin-right: 8px;
              .btn-img {
                width: 14px;
                height: 14px;
                position: relative;
                top: 1px;
              }
            }
          }
        }
        .col2 {
          width: 30%;
          padding: 0 10px 0 10px;
          .label {
            color: #fff;
            font-size: 16px;
          }
          .item {
            margin-top: 20px;
            color: rgba(255, 255, 255, 0.6);
            font-size: 12px;
          }
        }
        .col3 {
          width: 30%;
          padding: 0 5px;
          .label {
            color: #fff;
            font-size: 16px;
          }
          .item {
            margin-top: 20px;
            color: rgba(255, 255, 255, 0.6);
            font-size: 12px;
          }
        }
        .col4 {
          width: 30%;
          .label {
            color: #fff;
            font-size: 16px;
            margin-bottom: 16px;
          }
        }
      }
    }

    .split-line {
      width: 100%;
      height: 1px;
      background-color: rgba(255, 255, 255, 0.6);
    }

    .copyright {
      padding: 15px 0;
      color: #adadad;
      font-size: 12px;
      text-align: center;
    }
  }
}
</style>
