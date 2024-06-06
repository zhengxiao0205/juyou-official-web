<template>
  <div class="form-wrapper">
    <div class="element-container form">
      <h3 class="title1">掌握更可靠的商业信息，抓住成长股投资机会</h3>
      <h6 class="title2">免费报名90分钟线上【投资分享会】</h6>
      <div class="enroll-form">
        <div class="form-item first-row">
          <label class="label" for="first-name">First Name</label>
          <input class="input" placeholder="First Name" id="first-name" />
        </div>
        <div class="form-item first-row">
          <label class="label" for="last-name">Last Name</label>
          <input class="input" placeholder="Last Name" id="last-name" />
        </div>
        <div class="form-item">
          <label class="label" for="facebook-name">Facebook Name</label>
          <input class="input" placeholder="我们需要Facebook Name批准您进群" id="facebook-name" />
        </div>
        <div class="form-item">
          <label class="label" for="email">Email</label>
          <input class="input" placeholder="Email Address" id="email" />
        </div>
        <div class="form-item">
          <label class="label" for="phone">Phone/Mobile</label>
          <input class="input" placeholder="012-345 6789" id="phone" />
        </div>
        <div class="form-item">
          <label class="label">投资经验</label>
          <div class="radio-item">
            <input type="radio" />
            <label class="radio-label">还没开始</label>
          </div>
          <div class="radio-item">
            <input type="radio" />
            <label class="radio-label">少过一年</label>
          </div>
          <div class="radio-item">
            <input type="radio" />
            <label class="radio-label">超过一年</label>
          </div>
        </div>
        <div class="form-item">
          <label class="label">碰到的问题</label>
          <div class="radio-item">
            <input type="radio" />
            <label class="radio-label">不会 Cut Loss</label>
          </div>
          <div class="radio-item">
            <input type="radio" />
            <label class="radio-label">不会选好公司</label>
          </div>
          <div class="radio-item">
            <input type="radio" />
            <label class="radio-label">经常被消息影响</label>
          </div>
          <div class="radio-item">
            <input type="radio" />
            <label class="radio-label">自己摸索找不到方向</label>
          </div>
          <div class="radio-item">
            <input type="radio" />
            <label class="radio-label">做股票做到很累，想要轻松的方法</label>
          </div>
          <div class="radio-item">
            <input type="radio" />
            <label class="radio-label">还没开始投资</label>
          </div>
        </div>
        <div class="submit-button">Submit Form</div>
      </div>
    </div>
  </div>
</template>

<script setup></script>

<style lang="less" scoped>
.form-wrapper {
  padding: 60px 0px 60px 0px;
  background-image: url('@/assets/images/enroll1.jpg');
  background-size: cover;
  .form {
    display: flex;
    flex-direction: column;
    align-items: center;

    .title1 {
      color: #fff;
      font-size: 44px;
    }

    .title2 {
      margin-top: 20px;
      color: #fff;
      font-size: 35px;
    }

    .enroll-form {
      width: 100%;
      display: flex;
      flex-wrap: wrap;
      margin-top: 30px;
      .form-item {
        display: flex;
        flex-direction: column;
        width: 100%;
        padding: 10px 20px;

        &.first-row {
          width: 50%;
          box-sizing: border-box;
        }

        .label {
          color: #fff;
          &:after {
            content: '*';
            color: #f56c6c;
            margin-left: 3px;
          }
        }

        .input {
          margin-top: 6px;
          width: 100%;
          outline: none; // 去除选中状态边框
          border: 1px solid #ced4da;
          border-radius: 4px;
          color: #495057;
          font-size: 16px;
          padding: 8px 12px;
        }

        .radio-item {
          margin-top: 2px;
          .radio-label {
            color: #fff;
          }
        }
      }

      .submit-button {
        background-color: #409eff;
        color: #fff;
        cursor: pointer;
        padding: 8px 15px;
        border-radius: 5px;
        margin-top: 15px;
        margin-left: 15px;
      }
    }
  }
}

// 移动端适配
@media (max-width: 600px) {
  .form-wrapper {
    padding: 60px 0px 60px 0px;
    background-image: url('@/assets/images/enroll1.jpg');
    background-size: cover;
    .form {
      display: flex;
      flex-direction: column;
      align-items: center;

      .title1 {
        color: #fff;
        font-size: 30px;
        text-align: center;
      }

      .title2 {
        margin-top: 20px;
        color: #fff;
        font-size: 28px;
        text-align: center;

      }

      .enroll-form {
        width: 100%;
        display: flex;
        flex-wrap: wrap;
        margin-top: 30px;
        .form-item {
          display: flex;
          flex-direction: column;
          width: 100%;
          padding: 10px 20px;

          &.first-row {
            width: 100%;
            box-sizing: border-box;
          }

          .label {
            color: #fff;
            &:after {
              content: '*';
              color: #f56c6c;
              margin-left: 3px;
            }
          }

          .input {
            margin-top: 6px;
            width: 90%;
            outline: none; // 去除选中状态边框
            border: 1px solid #ced4da;
            border-radius: 4px;
            color: #495057;
            font-size: 16px;
            padding: 8px 12px;
          }

          .radio-item {
            margin-top: 2px;
            .radio-label {
              color: #fff;
            }
          }
        }

        .submit-button {
          background-color: #409eff;
          color: #fff;
          cursor: pointer;
          padding: 8px 15px;
          border-radius: 5px;
          margin-top: 15px;
          margin-left: 15px;
        }
      }
    }
  }
}
</style>
