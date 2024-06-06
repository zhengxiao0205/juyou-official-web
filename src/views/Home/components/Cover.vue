<template>
  <div class="cover-wrapper">
    <div class="element-container cover PC">
      <img src="@/assets/images/cover-text.png" class="cover-text" />
      <p class="text">用商业情报，挖掘成长股</p>
    </div>
    <div class="mobile">
      <img src="@/assets/images/cover1.jpg" class="mobile-img" />
    </div>
  </div>
</template>

<script setup></script>

<style lang="less" scoped>
.cover-wrapper {
  background-color: #1399d3;
  background-image: url('@/assets/images/cover.jpg');
  background-position: center center;
  background-size: cover;
  .cover {
    min-height: 70vh;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    .cover-text {
      width: 60%;
    }

    .text {
      font-size: 46px;
      color: #fff;
      font-weight: bold;
      margin: 0;
    }
  }
}

.mobile {
  display: none;
}

// 移动端适配
@media (max-width: 600px) {
  .cover-wrapper {
    background-image: none;
    background-color: transparent;
  }
  .PC {
    display: none !important;
  }
  .mobile {
    display: block;
    .mobile-img {
      width: 100%;
    }
  }
}
</style>
