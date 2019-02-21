<template>
  <div class="backtop-section">
    <a href="https://udn.com/upf/ubrand/2019_data/DaretoDream/index.html">
      <div class="backtop-btn" :class="{ 'backtop-active': isActive}">
        <img :src="home" alt="">
        <p>HOME</p>
      </div>
    </a>   
  </div>
</template>

<script>
import setProps from '@/mixin/setProps.js'
import Utils from 'udn-newmedia-utils'
export default {
  name: 'BackTop',
  mixins: [ setProps ],
  data () {
    return {
      isActive: true,
      home: require('@/../static/homeWeb.png')
    }
  },
  props: {
    arrowColor: {
      type: String,
      default: '#fff'
    },
    arrowBoxColor: {
      type: String,
      default: '#E5E5E5'
    },
    jsonProps: {
      type: Object,
      default: null
    }
  },
  methods: {
    handle_scroll () {
      let currentH = window.pageYOffset
      if (currentH > window.innerHeight) {
        this.isActive = false
      } else {
        this.isActive = true
      }
    }
  },
  mounted () {
    window.addEventListener('scroll', this.handle_scroll)
  },
  destroyed () {
    window.removeEventListener('scroll', this.handle_scroll)
  }
}
</script>

<style lang="scss" scoped>
.backtop-section{
  position: fixed;
  z-index: 300;
  right: 10px;
  bottom: 10px;
  width: 45px;
  height: 45px;
  overflow: hidden;
  @media screen and (max-width: 767px) {
    display: none;
  }
  @media screen and (min-width: 768px) and (max-width: 1023px) {
    bottom: 60px;
  }
  @media screen and (min-width: 1025px) {
    bottom: 10vh;
    right: 50%;
    margin-right: -520px;
  }
  a {
    text-decoration: none;
  }
  .backtop-btn{
    width: 45px;
    height: 45px;
    display: flex;
    align-items: center;
    justify-content: center;
    background-color: #e60414;
    cursor: pointer;
    transition: 333ms ease;
    transform: translate3d(0, 0, 0);
    flex-direction: column;
    @media screen and (min-width: 768px) and (max-width: 1023px) {
      bottom: 60px;
    }
    p {
      font-size: 8px;
      color: #fff;
      margin: 0;
      @media screen and (min-width: 768px) and (max-width: 1023px) {
        line-height: 1;
      }
    }
  }
  .backtop-active{
    transform: translate3d(0, 100%, 0);
  }
}


</style>
