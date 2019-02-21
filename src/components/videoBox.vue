<template>
  <div class="videoBox">
    <youtube :src="videoInfo.video"></youtube>
    <div class="content">
        <div :style="{'background-image': 'url(' + videoInfo.img + ')' }" class="flag">
            <h3>{{ videoInfo.number }}</h3>
        </div>
        <h5><div v-html="videoInfo.slogan"></div></h5>
    </div>
  </div>
</template>

<script>
import youtube from '@/components/base/Youtube.vue'
export default {
  name: 'videoBox',
  data () {
    return {

    }
  },
  props: {
    videoInfo: Object
  },
  components: {
    youtube
  },
}
</script>

<style lang="scss" scoped>
.videoBox{
  .content {
      height: 100px;
      position: relative;
      display: -webkit-flex;
      display: flex;
      -webkit-align-items: center;
      align-items: center;
      -webkit-justify-content: center;
      justify-content: center;
      .flag {
          width: 30%;
          height: 100%;
          position: absolute;
          left: 0;
          background-position: center;
          background-repeat: no-repeat;
          background-size: cover;
        h3 {
            margin: 0px;
            padding: 0px;
            color: white;
            font-size: 35px;
            padding: 7px;
        }
      }

      h5 {
          margin: 0;
          padding: 0;
          line-height: 1.07;
          font-family: 微軟正黑體;
          font-weight: bold;
          letter-spacing: -0.6px;
          font-size: 21px;
      }
  }
}
</style>
