<template>
  <div id="app">
    <indicator></indicator>
    <div class="cover" :style="{'background-image': 'url(' + srcRWD(cover, coverWeb) + ')' }">
      <!-- <img :src="srcRWD(cover, coverWeb)" alt="" class="main-cover"> -->
      <div class="cover-title">
        <h3>
          Duncan：有生之年<br>要畫出一幅讓世界看見的作品
        </h3>
      </div>
    </div>
    <div class="back-to-home" ref="home" :class="{ 'hidden-home' : isShowHome }">
      <a class="home" href="https://udn.com/upf/ubrand/2019_data/DaretoDream/index.html">
        <img :src="srcRWD(home, homeWeb)" alt="">
        HOME
      </a>
    </div>
    <br>
    <content-container>
      <share href="https://udn.com/upf/ubrand/2019_data/DaretoDream_Duncan/index.html"></share>
      <br>
      <div class="title-track-same-month">
         <youtube src="https://www.youtube.com/embed/GwF4fFnxTkg"></youtube>
      </div>
      <br>
      <p>眼前的是在臉書擁有320萬粉絲的圖文界天王Duncan，公開場合總是戴著一張黑白面具，他的作品從公車、捷運、食物包裝、手搖杯到桌遊都看得到，至今出道五年，即便其他圖文插畫家如雨後春筍般出現，仍難以撼動他在圖文界的地位。</p>
      <br>
      <p>走進Duncan房間，除了滿滿的插畫、周邊作品，最多的就是星際大戰商品，記者忍不住問：「星際大戰跟插畫，你比較愛哪個？」，他秒回「這根本就是媽媽跟女友掉進水裡的問題吧！」引起一陣哄堂大笑。真性情的Duncan就像鄰家大男孩，講到夢想，他仍不忘初心，不管是商業案或日常創作，堅持畫自己想畫的，並堅信「帶給大家快樂」這個理念。</p>
      <br>
      <column-one description="Duncan 房間內除了自創作品，還有滿滿的星際大戰商品。" src="@/../static/pic1.png" src-web="@/../static/pic1_web.png"></Column-One>
      <br>
      <h3>插畫不一定要有梗　<br class="mobile-only">只要有Fu</h3>
      <br>
      <p>剛開始創作的幾年，Duncan堅持「一日一po文」。談到創作靈感，他說，「我有一個職業病是，走到哪裡都會想這個可以畫、那個可以畫，看到路邊坐了某個人，我就拿手機出來把他記在記事本。」那怎麼挑選要畫哪些？「看心情！有時候看到這idea會覺得，像我今天的狀態(心情)，我就趕快把它挑起來畫，在你有感的當下，寫出來的文字也會是有感的。」Duncan認為，只要能給讀者「一個感覺」，不論正能量或負能量，他都不避諱跟讀者分享。</p>
      <br>
      <p>被問到會不會有疲憊的時候，Duncan則強調：<b>「千萬不要把自己最愛的事變成例行公事。」</b>他舉例，「你很喜歡吃日本料理，但每天吃一定也會覺得，哇，會累會怕，那當然畫圖也是。」因此對於畫圖，他更小心謹慎地呵護這個夢想。</p>
      <br>
      <column-one description="Duncan 筆下主角，經典西瓜皮、黑框眼鏡和法令紋，是大家最熟知的插畫角色。" src="@/../static/pic2.png" src-web="@/../static/pic2_web.png"></Column-One>
      <br>
      <h3>多種打工經驗　<br class="mobile-only">反倒成為創作養分</h3>
      <br>
      <p>Duncan也有過迷惘的時刻。因為父親反對他將畫畫當志向，使他就學時期無法選擇美術相關科系，等到大學畢業後，Duncan自覺關於畫畫這件事，已落後同年齡的人大半拍。他後來索性把畫畫當作興趣，擺過地攤，當過英文老師、餐廳服務生、民宿櫃台、軟體公司美工，「我當時就是抱著『沒有人看，我自己畫還是很開心』的態度，可是飯還是要先吃飽，要不然什麼事情都不用談了。」</p>
      <br>
      <p>他認為，「至少有錢讓自己生活，即使你做的並不是最喜歡的工作；<b>如果真的這麼喜歡某一件事，那你應該可以在工作之餘騰出時間去做這件事，而且是不計回報的去做。</b>」</p>
      <br>
      <p>就是這份堅持，讓Duncan在其他工作經驗中慢慢累積養分，擺地攤就是很特別的經歷，「我本身不是一個很外放的人，但擺攤因為工作需要，我可以跟陌生人大吼大叫，或逗他們笑，也許是因為這些不同的工作經驗，讓我現在的作品可以比較不一樣。」</p>
      <br>
      <column-one description="Duncan 隨身公仔，IG、Facebook上常看到他的蹤影。" src="@/../static/pic3.png" src-web="@/../static/pic3_web.png"></Column-One>
      <br>
      <h3>把大夢想拆成小夢想　<br class="mobile-only">逐步實踐</h3>
      <br>
      <p>Duncan有句名言是：「夢想再高，你還是碰得到！」那夢想要如何碰到？「我會把夢想拆成很多小的、可以理解的範圍。」他舉例，「我希望一年後可以請我媽吃一頓飯，這是很小的夢想，當你達成的時候，就會想到下一個『我希望可以請全家人吃一頓飯』。」對他來說，夢想並非遙不可及，而是學會在日常中一一實踐。</p>
      <br>
      </content-container>
      <content-container class="web-only" style="background-image: linear-gradient(to bottom, #f2f2f2, rgba(255, 255, 255, 0)); ">
      <div class="anchor-web">
        <h3 class="anchor-web-title">點看其他人物故事</h3>
        <ul>
          <li v-for="item in profiles" :key="item.id"  :class="{ shake: item.isLock }" >
            <a :href="item.link">
              <img :src="item.profile_web" @click="handleLinkTo(item.isLock, item.idTo, $event)" alt="">
              <div class="describe">
                <p>{{ item.title }}</p>
                <p>{{ item.name }}</p>
             </div>
            </a>
          </li>
        </ul>
      </div>
      </content-container>
      <div class="anchor-mobile">
        <h3 class="anchor-mobile-title">點看其他人物故事</h3>
        <ul>
          <li v-for="item in profiles" :key="item.id" :class="{ shake: item.isLock }">
            <a :href="item.link">
              <img :src="item.profile" @click="handleLinkTo(item.isLock, item.idTo, $event)" alt=""  >
              <div class="describe">
                <p>{{ item.title }}</p>
                <p>{{ item.name }}</p>
             </div>
            </a>
          </li>
        </ul>
      </div>
      <content-container>
      <br>
      <div class="share-and-logo"> 
        <div class="share">
          <share href="https://udn.com/upf/ubrand/2019_data/DaretoDream_Duncan/index.html"></share>
        </div>
        <div class="logo">
          <logo use-ubrand="yes" use-vision='no'>
            <div>
              <img :src="logo" alt="">
            </div>         
          </logo>
        </div>
      </div>
      <p><br></p>
      <editor>
        <div>文字採訪：盧巧梅</div>
        <div>影音製作：劉宜峰</div>
        <div>視覺設計：呂宗原</div>
        <div>網頁製作：胡凈悟</div>
        <div>議題行銷：張乃文、陳欣媛、王敏霏</div>
        <div>監製：潘如瑩、董谷音、蔡幸怡、陳曼薇</div>
        <div>2019.2.15</div>
      </editor>
      <p><br></p>
      <fb-comment href="https://udn.com/upf/ubrand/2019_data/DaretoDream_Duncan/index.html"></fb-comment>
    </content-container>
    <back-home></back-home>
    <back-top></back-top>
    <foot></foot>
  </div>
</template>

<script>
import Vue from 'vue'
import srcRWD from '@/mixin/srcRWD.js'
import globalComponents from '@/plugins/baseComponents.js'
import videoBox from '@/components/videoBox.vue'
import backHome from '@/components/backHome.vue'

Vue.use(globalComponents)

export default {
  name: 'App',
  mixins: [srcRWD],
  components: {
    videoBox,
    backHome
  },
  data () {
    return {
      isShowHome: false,
      cover: require('@/../static/cover.png'),
      coverWeb: require('@/../static/cover_web.png'),
      logo: require('@/../static/logo.png'),
      home: require('@/../static/home.png'),
      homeWeb: require('@/../static/homeWeb.png'),
      profiles: [
      {
        id: 'duncan_btn',
        idTo: 'duncan',
        title: '圖文創作者',
        name: 'Duncan',
        profile: require('@/../static/profiles/duncan.png'),
        profile_web: require('@/../static/profiles/duncan_web.png'),
        link: 'https://udn.com/upf/ubrand/2019_data/DaretoDream_Duncan/index.html',
        isLock: false
      },
      {
        id: 'br_btn',
        idTo: 'br',
        title: '饒舌歌手',
        name: 'BR',
        profile: require('@/../static/profiles/br.png'),
        profile_web: require('@/../static/profiles/br_web.png'),
        link: 'https://udn.com/upf/ubrand/2019_data/DaretoDream_BR/index.html',
        isLock: false
      },
      {
        id: 'anonymous1_btn',
        idTo: 'anonymous1',
        title: '3月',
        name: '即將推出',
        profile: require('@/../static/profiles/lock.png'),
        profile_web: require('@/../static/profiles/lock_web.png'),
        link: '.',
        isLock: true
      },
      {
        id: 'anonymous2_btn',
        idTo: 'anonymous2',
        title: '4月',
        name: '即將推出',
        profile: require('@/../static/profiles/lock.png'),
        profile_web: require('@/../static/profiles/lock_web.png'),
        link: '.',
        isLock: true
      },
      {
        id: 'anonymous3_btn',
        idTo: 'anonymous3',
        title: '5月',
        name: '即將推出',
        profile: require('@/../static/profiles/lock.png'),
        profile_web: require('@/../static/profiles/lock_web.png'),
        link: '.',
        isLock: true
      },
      {
        id: 'anonymous4_btn',
        idTo: 'anonymous4',
        title: '6月',
        name: '即將推出',
        profile: require('@/../static/profiles/lock.png'),
        profile_web: require('@/../static/profiles/lock_web.png'),
        link: '.',
        isLock: true
      }]
    }
  },
  methods: {
    handleLinkTo (isLock ,idTo ,event) {
      
      let label = "[DaretoDream_Duncan][" + idTo + "][外連到" + idTo + "]"

      if(isLock) {
        label = "[DaretoDream_Duncan][" + idTo + "][目前無法外連]"
        event.preventDefault()
      }
      
      window.ga("ubrand.send", {
        "hitType": "event",
        "eventCategory": "OptionButton",
        "eventAction": "click",
        "eventLabel": label
      })

      console.log("It will send label:" + label)
    },
    handle_scroll () {
      let currentHeight = window.pageYOffset
      if (currentHeight > 0) {
        this.isShowHome = true
      } else {
        this.isShowHome = false
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

<style  lang="scss">
@import './assets/CSS/theme.css';
@import './assets/CSS/UdnFontSize.css';

html, body {
  margin: 0;
  padding: 0;
}
#app {
  font-family: Microsoft JhengHei;
    .web-only {
      @media screen and (max-width: 768px) {
        display: none;
      }
      @media screen and (min-width: 768px) and (max-width: 1023px) {
          display: none;
      }
    }
    .mobile-only {
        @media screen and (min-width: 768px) and (max-width: 1023px) {
          display: none;
        }
        @media screen and (min-width: 1024px) {
          display: none;
        }
      }
    .cover {
      position: relative;
      background-repeat: no-repeat;
      background-size: cover;
      background-position: center;
      height: 100vh;
       @media screen and (min-width: 1440px) {
          height: 100vh;
        }
      .main-cover {
        width: 100%;
      } 
      .cover-title {
        width: 100%;
        background-color: rgba(#e60414, 0.6);
        position: absolute;
        bottom: 110px;
        left: 0;
        @media screen and (min-width: 768px) and (max-width: 1023px) {
          bottom: 0;
        }
        @media screen and (min-width: 1024px) {
          bottom: 0;
        }
        h3 {
          margin: 0px;
          padding: 9px 15px 12px 15px;
          color: white;
          font-weight: bolder;
          @media screen and (min-width: 768px) and (max-width: 1023px) {
            font-size: 5vw;
            padding: 9px 50px 12px 50px;
          }
          @media screen and (min-width: 1024px) {
            font-size: 5vw;
            padding: 9px 50px 12px 50px;
          }
        }
      }
    }
    .back-to-home {
      width: 48px;
      height: 47px;
      background-color: #e60414;
      border-radius: 51% 0 0 51%;
      padding: 10px;
      position: fixed;
      right: 0;
      bottom: 10vh;
      z-index: 100;
      font-size: 9px;
      white-space: nowrap;
      cursor: pointer;
      display: flex;
      align-items: center;
      transform: translateX(100%);
      opacity: 0;
      transition: all 1s;
      font-weight: 900;
      @media screen and (min-width: 768px) and (max-width: 1023px) {
        display: none;
      }
      @media screen and (min-width: 1024px) {
        display: none;
      }
      a {
        color: white;
        cursor: pointer;
        width: 100%;
        height: 100%;
        img {
          display: block;
          width: 9px;
          position: relative;
          left: 50%;
          transform: translate(-25%);
        }
      }
    }
    .hidden-home {
      transform: translateX(0%);
      opacity: 1;
    }
    .anchor-web {
      @media screen and (max-width: 768px) {
        display: none;
      }
      .anchor-web-title {
        padding: 21px 0 55px 0;
        font-size: 37.9px;
        font-weight: bold;
        text-align: center;
      }
      ul {
        display: flex;
        justify-content: space-around;
        margin:0;
        padding: 0;
        text-indent: 0;
        list-style-type: 0;
        li {
          overflow: hidden;
          height: auto;
          width: 110px;
          display: flex;
          align-items: center;
          justify-content: center;
          flex-direction: column;
          position: relative;
          a {
            text-decoration: none;
            color: black;
            width: 100%;
          }
          img {
            width: 100%;
            min-width: 110px;
            cursor: pointer;
            border-radius: 51%;
          }
          p {
            margin: 0;
            line-height: 1;
            text-align: center;
            font-size: 17px;
            line-height: 1.35;
            font-weight: bolder;
          }
          .locked {
            background-color: gray;
            width: 100%;
            height: 100%;
            position: absolute;
          }
        }
        .shake:hover, .shake:active {
            animation: shake 0.82s cubic-bezier(.36,.07,.19,.97) both;
            transform: translate3d(0, 0, 0);
            backface-visibility: hidden;
            perspective: 1000px;
          }
          @keyframes shake {
            10%, 90% {
              transform: translate3d(-1px, 0, 0);
            }
            
            20%, 80% {
              transform: translate3d(2px, 0, 0);
            }

            30%, 50%, 70% {
              transform: translate3d(-4px, 0, 0);
            }

            40%, 60% {
              transform: translate3d(4px, 0, 0);
            }
          }
      }
    }
   .anchor-mobile {
     background-image: linear-gradient(to bottom, #f2f2f2, rgba(255, 255, 255, 0));
     padding-bottom: 13px;
      @media screen and (min-width: 1024px) {
        display: none;
      }
      .anchor-mobile-title {
        padding: 25px 0;
        font-size: 25px;
        font-weight: 900;
        text-align: center;
        color: black;
        margin: 0;
        text-align: center;
      }
      ul {
        display: flex;
        flex-wrap: wrap;
        justify-content: space-around;
        margin:0;
        padding: 0;
        text-indent: 0;
        list-style-type: 0;
        li {    
          overflow: hidden;
          width: 30%;
          display: flex;
          align-items: center;
          justify-content: center;
          position: relative;
          margin: 5px 0;
          flex-direction: column;
          text-align: center;
          @media screen and (min-width: 768px) and (max-width: 1023px) {
            width: 15%;
            height: auto;
          }
          a {
            text-decoration: none;
            color: black;
            width: 100%;
          }
          img {
            width: 75%;
            cursor: pointer;
            border-radius: 51%;
            margin: 5px;
          }
          p {
            margin: 0;
            line-height: 1;
            text-align: center;
            font-size: 12px;
            line-height: 1.33;
            font-weight: bolder;
          }
          .locked {
            background-color: gray;
            width: 100%;
            height: 100%;
            position: absolute;
          }
        }
        .shake:hover, .shake:active {
            animation: shake 0.82s cubic-bezier(.36,.07,.19,.97) both;
            transform: translate3d(0, 0, 0);
            backface-visibility: hidden;
            perspective: 1000px;
          }
          @keyframes shake {
            10%, 90% {
              transform: translate3d(-1px, 0, 0);
            }
            
            20%, 80% {
              transform: translate3d(2px, 0, 0);
            }

            30%, 50%, 70% {
              transform: translate3d(-4px, 0, 0);
            }

            40%, 60% {
              transform: translate3d(4px, 0, 0);
            }
          }
      }
    }
    .share-and-logo {
      display: flex;
      justify-content: flex-start;
      flex-direction: column;
      @media (min-width: 768px) and (max-width: 1024px){
        justify-content: space-between;
        flex-direction: row;
      }
      @media screen and (min-width: 1025px){
        justify-content: space-between;
        flex-direction: row;
      }
      .share {
        min-width: 35%;
      }
      .logo {
        @media (min-width: 768px) and (max-width: 1024px){
          margin-top: -5px;
        }
        @media screen and (min-width: 1025px){
          margin-top: -5px;
        }
      }
    }
}
</style>
