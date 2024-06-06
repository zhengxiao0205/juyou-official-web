<template>
  <div class="navbar-wrapper">
    <div class="fixed PC">
      <div class="navbar">
        <img src="@/assets/images/logo.jpg" class="logo" />
        <div class="right">
          <div class="nav-items">
            <div class="item">Events</div>
            <div class="item">Free Contents</div>
            <div class="item">How to Maximize Wealth</div>
            <div class="item">Grow Savings</div>
            <div class="item">About us</div>
            <div class="item">Purchase</div>
            <div class="item">Courses</div>
            <div class="item">EN</div>
          </div>

          <div class="split-line"></div>
          <div class="login-button">
            <img src="@/assets/images/person.png" class="login-img" />
            <span>Login</span>
          </div>
          <div class="cart">
            <img src="@/assets/images/cart.png" class="cart-img" />
            <div class="cart-number">0</div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup></script>

<style lang="less" scoped>
.navbar-wrapper {
  height: 80px;
  .fixed {
    position: fixed;
    left: 0;
    right: 0;
    background-color: #fff;
    z-index: 1000;

    .navbar {
      max-width: 1242px;
      height: 80px;
      margin: 0 auto;
      display: flex;
      align-items: center;
      justify-content: space-between;

      .logo {
        width: 160px;
        height: 64px;
      }

      .right {
        display: flex;
        align-items: center;
        .nav-items {
          display: flex;
          align-items: center;
          flex-wrap: wrap;
          .item {
            font-size: 15px;
            color: #4a5568;
            cursor: pointer;
            padding: 9px;
            &:hover {
              color: #2b6cb0;
            }
          }
        }

        .split-line {
          background-color: #718096;
          height: 40px;
          width: 1px;
          margin: 0 10px;
        }

        .login-button {
          display: flex;
          align-items: center;
          cursor: pointer;
          margin-right: 10px;
          .login-img {
            width: 18px;
            height: 18px;
            margin-right: 3px;
          }
        }

        .cart {
          display: flex;
          align-items: center;
          cursor: pointer;
          .cart-img {
            width: 20px;
            height: 20px;
            margin-right: 3px;
          }
          .cart-number {
            width: 20px;
            height: 20px;
            border-radius: 50%;
            background-color: #edf2f7;
            display: flex;
            justify-content: center;
            align-items: center;
            font-size: 12px;
            color: #666;
          }
        }
      }
    }
  }
}

// 移动端适配
@media (max-width: 600px) {
  .navbar {
    padding: 0 20px;
  }
  .fixed {
    position: relative !important;
  }

  .nav-items {
    display: none !important;
  }

  .split-line {
    display: none !important;
  }
}
</style>
