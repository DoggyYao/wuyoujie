<template>
  <div class="home">
    <div class="logo">
      <img src="../assets/image/home-page-bg1.jpg" alt="">
    </div>

    <div class="btn-container">
      <div class="first-box">
        <!-- 直播间 -->
        <section class="zhibojian" @click="go('live')">
          <div class="entrance">
            <img src="../assets/image/zhibojian.png" alt="">
          </div>
          <div class="title">直播间</div>
        </section>

        <!-- 注册报名 -->
        <section class="zhucebaoming" @click="go('register')">
          <div class="entrance">
            <img src="../assets/image/zhucebaoming.png" alt="">
          </div>
          <div class="title">注册报名</div>
        </section>
      </div>

      <div class="second-box">
        <!-- 欢迎辞 -->
        <section class="huanyingci" @click="go('helloWord')">
          <div class="entrance">
            <img src="../assets/image/huanyingci.png" alt="">
          </div>
          <div class="title">欢迎辞</div>
        </section>

        <!-- 组织架构 -->
        <section class="zuzhijiagou" @click="go('zuzhijiagou')">
          <div class="entrance">
            <img src="../assets/image/zuzhijiagou.png" alt="">
          </div>
          <div class="title">组织架构</div>
        </section>

        <!-- 会议日程 -->
        <section class="huiyiricheng" @click="go('huiyiricheng')">
          <div class="entrance">
            <img src="../assets/image/huiyiricheng.png" alt="">
          </div>
          <div class="title">会议日程</div>
        </section>
      </div>

      <div class="third-box">
        <!-- 云展厅 -->
        <section class="yunzhanting" @click="go('yunzhanting')">
          <div class="entrance">
            <img src="../assets/image/yunzhanting.png" alt="">
          </div>
          <div class="title">云展厅</div>
        </section>

        <!-- 会议信息 -->
        <section class="huiyixinxi" @click="go('huiyixinxi')">
          <div class="entrance">
            <img src="../assets/image/huiyixinxi.png" alt="">
          </div>
          <div class="title">会议信息</div>
        </section>

        <!-- 学分领取 -->
        <section class="xuefenlingqu" @click="go('xuefenlingqu')">
          <div class="entrance">
            <img src="../assets/image/xuefenlingqu.png" alt="">
          </div>
          <div class="title">学分领取</div>
        </section>
      </div>
    </div>
  </div>
</template>

<style scoped>
.home {
  height: 100%;
}

.logo {
  width: 100%;
  height: 10rem;
}

.logo img {
  width: 100%;
  height: 100%;
  object-fit: fill;
}

.btn-container {
  width: 100%;
  margin-top: 3rem;
}

.first-box,
.second-box,
.third-box {
  width: 100%;
  padding: 1rem 2rem;
  display: flex;
  align-items: center;
  justify-content: space-around;
  box-sizing: border-box;
}

.zhibojian,
.zhucebaoming,
.huanyingci,
.zuzhijiagou,
.huiyiricheng,
.yunzhanting,
.huiyixinxi,
.xuefenlingqu {
  width: 5rem;
}

.zhibojian .entrance,
.zhucebaoming .entrance,
.huanyingci .entrance,
.zuzhijiagou .entrance,
.huiyiricheng .entrance,
.yunzhanting .entrance,
.huiyixinxi .entrance,
.xuefenlingqu .entrance  {
  width: 100%;
  height: 5rem;
}

.zhibojian .entrance img,
.zhucebaoming .entrance img,
.huanyingci .entrance img,
.zuzhijiagou .entrance img,
.huiyiricheng .entrance img,
.yunzhanting .entrance img,
.huiyixinxi .entrance img,
.xuefenlingqu .entrance img {
  width: 100%;
  height: 100%;
  object-fit: cover;
}

.zhibojian .title,
.zhucebaoming .title,
.huanyingci .title,
.zuzhijiagou .title,
.huiyiricheng .title,
.yunzhanting .title,
.huiyixinxi .title,
.xuefenlingqu .title {
  height: 2rem;
  line-height: 2rem;
  color: #133474;
  text-align: center;
  font-weight: 700;
  font-size: 1.125rem;
  margin-top: 0.25rem;
}

@media (min-width: 700px) and (max-width: 900px) {
  .logo {
    height: 18rem;
  }
}

@media (min-width: 901px) and (max-width: 1200px) {
  .logo {
    height: 24rem;
  }

  .first-box,
  .second-box,
  .third-box {
    padding: 2rem 5rem;
  }
}

@media (min-width: 1201px) and (max-width: 1500px) {
  .logo {
    height: 28rem;
  }

  .first-box,
  .second-box,
  .third-box {
    padding: 2rem 7rem;
  }
}

@media (min-width: 1501px) and (max-width: 2300px) {
  .logo {
    height: 32rem;
  }

  .first-box,
  .second-box,
  .third-box {
    padding: 2rem 7rem;
  }
}

@media (min-width: 2301px) and (max-width: 2500px) {
  .logo {
    height: 36rem;
  }

  .first-box,
  .second-box,
  .third-box {
    padding: 2rem 7rem;
  }
}


</style>

<script lang="ts">
import { Component, Vue } from 'vue-property-decorator';

@Component({
  components: {
  },
})
export default class Home extends Vue {
  [x: string]: any;

  mounted() {
    console.log('yaoyao-这是主页');
  }

  /**
   * 页面路由跳转
   */
  go(page: string) {
    this.$router.push(page);
  }

}
</script>
