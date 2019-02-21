<template>
  <div class="logo-block">
    <div class="thirdparty">
      <slot></slot>
    </div>
    <div class="logo" v-if="yesToBoolean(setProps('useVision'))">
      <a href="https://vision.udn.com/" target="_blank"><img width="140" src="https://udn.com/upf/newmedia/image/20180829Logo/logo_udnhope2.jpg" alt=""></a>
    </div>
    <div class="logo">
      <a href="https://udn.com/news/index" target="_blank"><img src="https://udn.com/upf/newmedia/image/20180829Logo/logo_udn2.jpg"></a>
    </div>
    <div class="logo" id="nmd" v-if="yesToBoolean(setProps('useUbrand'))">
      <a href="https://udn.com/upf/newmedia/ubrandstudio/" target="_blank"><img class="ubrain" :src="ubrain"></a>
    </div>
    <div class="logo" id="nmd" v-if="!yesToBoolean(setProps('useUbrand'))">
      <a href="https://www.facebook.com/udnNewMediaLab/" target="_blank"><img src="https://udn.com/upf/newmedia/image/20180829Logo/logo_new_media_center2.jpg"></a>
    </div>
  </div>
</template>

<script>
import yesToBoolean from '@/mixin/yesToBoolean.js'
import setProps from '@/mixin/setProps.js'
export default {
  name: 'Logo',
  data () {
    return {
      ubrain: require('@/../static/ubrain.png'),
      udnNews: require('@/../static/udnNews.png')
    }
  },
  mixins: [setProps, yesToBoolean],
  props: {
    jsonProps: {
      type: Object,
      default: null
    },
    useVision: {
      type: String
    },
    useUbrand: {
      type: String
    }
  },
  mounted () {
    console.log(this.useUbrand)
  }
}
</script>

<style lang="scss" scoped>
  .logo-block {
    width: 100%;
    display: flex;
    @media (min-width: 768px) and (max-width: 1024px){

    }
    @media screen and (min-width: 1025px){
      justify-content: flex-end;
    }
    
    .logo{
      width: 140px;
      display: inline-block;
      img{
        width: 100%;
        height: auto;
      }
    }
    .udnNews {
      margin-top: 14px;
      padding-right: 8px;
      @media (min-width: 768px) and (max-width: 1024px){
        margin-top: 16px;
      }
      @media screen and (min-width: 1025px){
        margin-top: 14px;
        margin-right: 8px;
      }
    }
    .ubrain {
      margin-top: 18px;
      @media (min-width: 768px) and (max-width: 1024px){
        margin-top: 20px;
      }
      @media screen and (min-width: 1025px){
        margin-top: 18px;
      }
    }
    .thirdparty {
      margin-top: 8px;
      text-align: right;
      width: 25%;
      @media (min-width: 768px) and (max-width: 1024px){
 
      }
      @media screen and (min-width: 1025px){
        width: 16%;
      }
      img{
       width: 100%;
       height: 100%;
      }
    }
  }
</style>
