<template lang="html">
    <div>
    <v-index></v-index>
  <div class="wrapper">
    <div class="intr">
        <div class="timer">
            <img src="../public/icons/dengji.png" alt="">
            <span>活动中心</span>
            <br>
            <small>今日听歌0分钟</small>
        </div>
        <div class="avatar">
            <img src="../public/icons/avatar.jpg" alt="">
        </div>
        <div class="vip">
            <img src="../public/icons/vvip.png" alt="">
            <span>会员中心</span>
            <br>
            <small>豪华绿钻首月9.9</small>
        </div>
    </div>
    <p class="username">{{username}}</p>
    <div class="intr-songs">
        <div class="t-intr-songs">
            <div class="t-intr-songs1">
                <router-link to="/total">
                  <img src="../public/icons/yinfu.png" alt="">
                  <p>本地音乐</p>
                </router-link> 
            </div>
            <div class="t-intr-songs1">
                <router-link to="/download">
                <img src="../public/icons/download.png" alt="">
                <p>下载音乐</p>
                </router-link>
            </div>
            <div class="t-intr-songs1">
                <router-link to="/musiclist">
                <img src="../public/icons/zuijin.png" alt="">
                <p>最近播放</p>
                </router-link>
            </div>       
        </div>
        <div class="b-intr-songs">
            <div class="b-intr-songs1">
                <img src="../public/icons/heart.png" alt="">
                <p>我喜欢</p>
                <small></small>
            </div>
            <div class="b-intr-songs1">
                <img src="../public/icons/cd.png" alt="">
                <p>已购音乐</p>
            </div>
            <div class="b-intr-songs1">
                <img src="../public/icons/paobu.png" alt="">
                <p>跑步电台</p>
            </div>
        </div>
    </div>
    <div class="blank"></div>
  </div>
  
  
  <div class="songlist">
      <span class="title">自建歌单1</span>
      <span class="title title1">|</span>
      <span class="title">收藏歌单2</span>
      <span class="title"><img src="../public/icons/tianjia.png"></span>
  </div>
  <router-link to="/like">
  <div class="list" >
      <img src="../public/icons/jay1.jpg" alt="">
      <div class="number">
          <p>歌单1</p>
          <small></small>
      </div>
  </div>
  <br>
    <div class="list">
      <img src="../public/icons/jay1.jpg" alt="">
      <div class="number">
          <p>歌单2</p>
          <small></small>
      </div>
  </div>
  </router-link>
  <div class="blank2">
      
  </div>
  </div>
</template>

<script>
import index from '@/components/index.vue'
export default {
    data () {
        return {
            intrShow: false,
            username: '马伸'
        }
    },
    components: {
        "v-index": index
    },
    methods: {
      intrshow () {
         this. intrShow = ! this.intrShow
      }
    }
}
</script>

<style lang="scss" scoped>
@import '../assets/style/header.scss';

</style>