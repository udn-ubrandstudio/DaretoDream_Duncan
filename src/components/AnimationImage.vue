<template>
  <div class="animation">
    <div class="content1" :ref="aniamtionRef1">
        
    </div>

    <div class="content2" :ref="aniamtionRef2" v-if="animationConfig2"></div>
    <div class="title_box">
      <div>
        <slot></slot>
      </div>
    </div>
    <div class="describe">
        <slot name="describe">

        </slot>
    </div>
  </div>
</template>

<script>
import lottie from 'lottie-web'

export default {
  name: 'App',
  data () {
    return {
      cover1: '',
      cover2: '',
    }
  },
  props: {
      aniamtionRef1: {
          type: String,
          default: ''
      },
      aniamtionRef2: {
          type: String,
          default: ''
      },
      animationConfig1: {
          type: Object,
          default: function () {
              return {
                  renderer: 'svg',
                  loop: false,
                  autoplay: true,
                  path: ''
              }
          }
      },
      animationConfig2: {
          type: Object,
          default: function () {
              return {}
          }
      }
  },
  components: {},
  mounted () {
    let vm = this
    let element1 = vm.$refs[vm.aniamtionRef1]
    let config1 = {}

    config1 = { 'container': element1, ...vm.animationConfig1 }
    vm.cover1 = lottie.loadAnimation(config1);

    if (vm.animationConfig2) {
        let element2 = vm.$refs[vm.aniamtionRef2]
        let config2 = {}
        config2 = { 'container': element2, ...vm.animationConfig2 }
        vm.cover2 = lottie.loadAnimation(config2);
    }
  }
}
</script>

<style lang="scss" scoped>
.animation {
    width: 100%;
    position: relative;
    .content1 {
        max-height: 100vh;
        z-index: 1;
    }
    .content2 {
        position: absolute;
        top: 50%;
        transform: translateY(-50%);
        top: 0;
        left: 0;
        z-index: 10;
    }
    .title_box {
        width: 100%;
        height: 100%;
        display: flex;
        padding: 0 7.7777%;
        position: absolute;
        top: 0;
        left: 0;
        z-index: 20;
        align-items: center;
        justify-content: flex-end;
    }
    .describe {
        position: absolute;
        width: 100%;
        text-align: left;
        bottom: -50px;
        left: 50%;
        transform: translate(-50%, 20%);
        z-index: 55;
        color: gray;
        @media (min-width: 768px) and (max-width: 1023px) {
            max-width: 880px;
        }
        @media screen and (min-width: 1024px) {
            max-width: 880px;
        }
        p {
            font-size: 14px;
            line-height: 1.5;
            margin: 0px 15px;
            @media (min-width: 768px) and (max-width: 1023px) {
                font-size: 18px;
                margin: 0px;
            }
            @media screen and (min-width: 1024px) {
                font-size: 18px;
                margin: 0px;
            }
        }
    }
       
}
</style>
