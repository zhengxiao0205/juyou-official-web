<template>
  <div class="thought-wrapper">
    <div class="element-container thought">
      <h3 class="thought-title">“看看以下毕业学员们的感想”</h3>
      <div @click="playVideo = true" v-if="!playVideo" class="video-wrapper">
        <img src="@/assets/images/play-video.png" class="play-img" />
        <img src="@/assets/images/thought1.jpg" class="thought-img" />
      </div>
      <iframe
        v-else
        class="video-wrapper"
        src="https://www.youtube.com/embed/sWCbBZoK6gU?controls=1&rel=0&playsinline=0&modestbranding=0&autoplay=0&enablejsapi=1&origin=https%3A%2F%2Fwww.grandpine.com&widgetid=1"
      ></iframe>
      <div class="swiper-container">
        <!-- https://swiperjs.com/vue -->
        <swiper
          :slides-per-view="swiperNum"
          :space-between="10"
          @swiper="onSwiper"
          @slideChange="onSlideChange"
        >
          <swiper-slide v-for="(item, index) of cards" :key="index">
            <div class="swiper-card">
              <p>
                <strong v-if="item.title">{{ item.title }}</strong>
              </p>
              <p>{{ item.content }}</p>
              <div class="person-info">
                <img :src="require(`@/assets/images/thought${index + 2}.jpg`)" class="avatar" />
                <div>
                  <div class="name">{{ item.name }}</div>
                  <div class="job">{{ item.job }}</div>
                </div>
              </div>
            </div>
          </swiper-slide>
        </swiper>
      </div>
      <h6 class="thought-title2">
        松大资本成立了20年，在这期间认识了不同种类的投资者：有律师、医生、老师、小贩、家庭主妇
      </h6>

      <h6 class="thought-title3">不同背景的学员来到 BIS 学会以下这套散户都能掌握赚钱的方法</h6>
    </div>
  </div>
</template>

<script setup>
import { Swiper, SwiperSlide } from 'swiper/vue'
import 'swiper/css'
import { ref, onMounted } from 'vue'

const playVideo = ref(false)

const swiperNum = ref(3)

const cards = [
  {
    title: '从BIS课程中，我发觉了自己在投资股票时有一颗贪欲强的“狐狸心”，',
    content:
      '而课程提醒，投资前专心做功课，选择有价值的股票，别太注重短期浮动，找出股票价格变化时的实际估值，来作是否值得进场的决定。放下贪找快钱的欲望，放下忌妒别人在某股中得到利益的比较心，才是投资的正道。',
    name: '骆荣福',
    job: '余仁生董事经理',
  },
  {
    title: 'It is truly a good program for learning to become a value investor.',
    content:
      'Mentors are very helpful. The course has changed my perspective in investment and reinforced my investment approach.',
    name: 'Peng Wen',
    job: '马来西亚5G特工队成员 华为瑞典首席工程师',
  },
  {
    title: '松大是学习价值投资股票的好地方。',
    content: '老师们都很有经验认真教学。我觉得这次上二十一天的付费网课有很大收获，超值得。谢谢松大的老师们。',
    name: 'Snow See',
    job: '律师',
  },
  {
    title: 'Very good coach from Grandpine, very supportive from Coach to Assistant coach, ',
    content: 'very happy to join this big family~ Value investing can be easier and clearer!',
    name: 'CK Loh',
    job: '飞机师',
  },
  {
    title: '',
    content:
      'BIS的课程设计就是步骤模似该如何做好投资决策。感谢老师们的用心，耐心和包容，並常常及时把我们拉回价值投资的的轨道上。投资本是不是容易，但是思想观念对了，方法用对了，成功率也就提高了！希望毕业的同学们，我们一起加油',
    name: 'Regine Khor',
    job: '',
  },
  {
    title: '',
    content:
      '今天终于上完了21天BIS课程。课程相当紧凑，尤其是要交功课的时间，更是紧张。不过，个人认为做功课很好，因为可以让我们自己更好的了解学习到的东西怎样去运用。老师很有耐心的讲解每个学员的功课。上完课后，会觉得应该怎样去看待及评估一家公司。明白股价和估值的差别。回更淡然的看待股价的波动。谢谢Grandpine。大家加油，希望大家可以做得更好。',
    name: 'Say Tech Wee',
    job: '',
  },
  {
    title: '',
    content:
      '终于上完了松大21天的BIS价值投资课程。上完课之后心态有所调整及改变。以前常常被股价波动影响心情，现在了解了股价是脆弱的。老师们有系统和高质量的教学模式，简单易懂。我领悟到投资股票是必须评估企业的现金流，商业价值，企业成长及管理团队，选对生意也要在对的估值买进。真的获益良多，希望我在未来的投资路上更上一层楼，达到真正的财务自由。谢谢松大老师们的认真指导！真心推荐松大价值投资教育平台',
    name: 'Say Tech Wee',
    job: '',
  },
  {
    title: '',
    content:
      '曾经在市场上找了俗称“价值投资”的老师也报名其他“价值导师”的课程和加入会员，结果在股市还是撞墙，其他老师也是拍拍屁股讲sorry没有买卖建议。在股市不要钱的经验永远是最贵的，多走了很多冤枉路，也亏掉了很多冤枉钱。后悔没有早一点报名BIS课程，希望Grandpine坚持扩展更多bve导师让坚持做价值投资的grandpine学员可以得到更多的value',
    name: 'Keith Tan',
    job: '-Bis Batch 15-',
  },
  {
    title: '',
    content:
      '以前听人家讲股票根本听不懂，有时候跟风乱买烧到手。 对于股票菜鸟而言，我坚信必须进修提升自己。这个MCO 3.0过得很充实，学海无涯。最后，希望大家都赚的盆满钵满！-Batch14-',
    name: 'Karman Woong',
    job: '-Bis Batch 14-',
  },
  {
    title: '',
    content:
      'Grandpine Capital 是一家很有水准的 business investment strategy education company。在短短的21天里我从连股票户口都没有的一个门外汉。经过3位老师们的教导，我真的学习了很多在股票市场里如何找到好捞的生意才做价值投资，让自己的钱可以多倍增长。如果你也像我一样想在股票市场里赚钱旦又不知道怎样开始，Grandpine Capital 是一个很好的学习平台。',
    name: 'Kong Yoke Chun',
    job: '',
  },
]

onMounted(() => {
  if (document.documentElement.clientWidth < 600) {
    swiperNum.value = 1
  }
  window.addEventListener('resize', () => {
    // 刷新dom

    if (document.documentElement.clientWidth < 600) {
      swiperNum.value = 1
    } else {
      swiperNum.value = 3
    }
  })
})

const onSwiper = (swiper) => {
  console.log(swiper)
}
const onSlideChange = () => {
  console.log('slide change')
}
</script>

<style lang="less" scoped>
.thought-wrapper {
  padding: 60px 0px 60px 0px;
  background-color: #f8f9fa;
  border-bottom: 1px solid #d6d6d6;
  .thought {
    display: flex;
    flex-direction: column;
    align-items: center;

    .thought-title {
      color: #000;
      font-size: 44px;
    }

    .thought-title2 {
      color: #000;
      font-size: 20px;
      font-weight: normal;
      margin-top: 30px;
    }

    .thought-title3 {
      margin-top: 30px;
      color: #000;
      font-size: 32px;
    }

    .video-wrapper {
      margin-top: 15px;
      border-radius: 10px;
      width: 1120px;
      height: 630px;
      display: flex;
      justify-content: center;
      align-items: center;
      position: relative;
      cursor: pointer;

      .thought-img {
        position: absolute;
        width: 100%;
        height: 100%;
      }

      .play-img {
        z-index: 10;
        width: 100px;
        height: 100px;
      }
    }

    .swiper-container {
      margin-top: 30px;
      width: 98%;
      .swiper-card {
        background-color: #ffffff;
        border: 1px solid #7c7c7c;
        border-radius: 10px;
        padding: 30px;
        height: 400px;
        user-select: none;
        display: flex;
        flex-direction: column;
        align-items: center;
        p {
          text-align: center;
        }
        .person-info {
          display: flex;
          align-items: center;
          justify-content: center;
          margin-top: 30px;
          .avatar {
            width: 78px;
            height: 78px;
            border-radius: 50%;
            margin-right: 10px;
          }
          .name {
            font-weight: bold;
          }
        }
      }
    }
  }
}

@media (max-width: 1200px) {
  .video-wrapper {
    width: 960px !important;
    height: 540px !important;
  }
}

// 移动端适配
@media (max-width: 600px) {
  .thought-wrapper {
    padding: 60px 0px 60px 0px;
    background-color: #f8f9fa;
    border-bottom: 1px solid #d6d6d6;
    .thought {
      display: flex;
      flex-direction: column;
      align-items: center;

      .thought-title {
        color: #000;
        font-size: 20px;
      }

      .thought-title2 {
        color: #000;
        font-size: 18px;
        font-weight: normal;
        margin-top: 30px;
        text-align: center;
      }

      .thought-title3 {
        margin-top: 30px;
        color: #000;
        font-size: 24px;
        text-align: center;
      }

      .video-wrapper {
        margin-top: 15px;
        border-radius: 10px;
        width: 95% !important;
        height: 225px !important;
        display: flex;
        justify-content: center;
        align-items: center;
        position: relative;
        cursor: pointer;

        .thought-img {
          position: absolute;
          width: 100%;
          height: 100%;
        }

        .play-img {
          z-index: 10;
          width: 80px;
          height: 80px;
        }
      }

      .swiper-container {
        margin-top: 30px;
        width: 88%;
        .swiper-card {
          background-color: #ffffff;
          border: 1px solid #7c7c7c;
          border-radius: 10px;
          padding: 30px 40px;
          height: 370px;
          user-select: none;
          display: flex;
          flex-direction: column;
          align-items: center;
          p {
            text-align: center;
          }
          .person-info {
            display: flex;
            align-items: center;
            justify-content: center;
            margin-top: 30px;
            .avatar {
              width: 78px;
              height: 78px;
              border-radius: 50%;
              margin-right: 10px;
            }
            .name {
              font-weight: bold;
            }
          }
        }
      }
    }
  }
}
</style>
