<template>
  <div id="app">
    <indicator></indicator>
    <head-bar>
      <a slot="logo" href="https://ubrand.udn.com/ubrand/index"></a>
      <a href="https://udn.com/upf/newmedia/2018_data/newedu/index.html">誰殺了想像力</a>
      <a href="https://udn.com/upf/newmedia/2018_data/newedu/future/index.html" target="_blanck">未來人才力</a>
    </head-bar>
    <animation-cover  :animationConfig1="srcRWD(coverMob1, coverWeb1)" aniamtionRef1="cover1">
      <h1 class="coverTitle1">誰殺了我的想像力</h1>
      <h2 class="coverTitle2">為什麼台灣需要教育創新？</h2>
    </animation-cover>
    <content-container style="background-color: black; color: white">
      <share href="https://udn.com/upf/newmedia/2018_data/newedu/index.html"></share>
      <p><br></p>
      <p>過去的傳統教育，就像一列教育生產線，一樣的教材、一樣的教法，教著不一樣的我們。</p>
      <p><br></p>
      <p>從小接受傳統教育的我們，成為什麼樣的大人？我們忌諱天馬行空，我們害怕與眾不同，儘管內心柔軟，但得隨著社會冷漠。</p>
      <p><br></p>
      <p>教育創新不是菁英家長、教育工作者才需關心的議題，它與我們的社會息息相關，越來越多教育工作者，他們蹲下傾聽孩子的聲音，在乎孩子的未來會長成什麼模樣。</p>
      <p><br></p>
      <p>他們眼中的教育創新，不需要很炫的科技工具、不需要新穎的教學法，只需要一顆以人為本的心。</p>
      <p><br></p>
      <Quote :img="quote" text="每一個人都有隱藏的能力，只是沒有適合的環境讓他開發出來，透過多元學習的方式，讓他們思考，不要等別人來拯救他們，讓自己有能力解決問題。" refer="—— 郭守正"></Quote>
      <p><br></p>
      <p><br></p>
      <h3 class="subtitle">別等待superman  靠自己找解方</h3>
      <p><br></p>
      <p>「百年樹人」不是一句簡單的話，需要投入大量人力以及龐大資金。這幾年創新教育百花齊放，永齡教育基金會這3年來陸續支持LIS線上教學平台、DFC Taiwan全球孩童創意行動挑戰、共玩創作、成功大學資訊工程系教授蘇文鈺，以及許多原創性的教育團隊。</p>
      <p><br></p>
      <p>「<span class="highlight">教育不是為了學習技能，而是練習自己如何解決問題，</span>」帶領永齡教育基金會投入創新教育領域的董事長郭守正，是4個孩子的父親，他最明白家長的焦慮、教育工作者的努力，以及放眼國際人才的需求。</p>
      <p><br></p>
      <p>郭守正以一部紀錄片《WAITING FOR SUPERMAN》（等待超人）為例說明，亞洲國家普遍都有waiting for superman的問題，總期待在位者、組織領導者提供願景與社會問題解方，而所有人就等待著被照顧。</p>
      <p><br></p>
      <p>但教育核心精神並非如此。郭守正強調，不管永齡教育基金會或是鴻海教育基金會，投資的教育團隊，初心都是如何引發孩子學習動機，以及引導孩子自己想解決方法。</p>
      <p><br></p>
      <p>「每一個人都有隱藏的能力，只是沒有適合的環境讓他開發出來，透過多元學習的方式，讓他們思考，不要等別人來拯救他們，讓自己有能力解決問題，」郭守正說，如果一個國家多數人有這樣的態度，那麼國家的人才也好、方向也好，一點都不需要擔心。</p>
      <p></p>
      <p><br></p>
    </content-container>
    <youtube :src="eductionVideo" showinfo="no" controls="yes" autoplay="no" muted="yes"></youtube>
    <content-container  style="background-color: black; color: white">
      <anchor title="教育像工廠">
        <div class="main-title" style="background-color: black; color: white">
          <h3 class="title" style="color: white">教育工廠製造的孩子</h3>
          <h3 class="title" style="color: white">缺乏不乖、表達自我、好奇的能力</h3>
          <ul>
            <li class="green-line"></li>
            <li class="red-line"></li>
            <li class="black-line"></li>
            <li class="light-green-line"></li>
          </ul>
        </div>
      </anchor>
      <p><br></p>
      <p>未來世代是AI人工智慧、資訊爆炸的世代，充滿變動與不可預測，<span class="highlight">我們卻還在用過去的方式教現代的孩子面對未來。</span></p>
      <p><br></p>
      <p>傳統教育為了工業時代的大量製造、集體工作準備，訓練團體的紀律與服從；傳統教育的優點是方便評分與比較，但已經無法培養孩子面對未來問題的能力。</p>
      <p><br></p>
      <p>全球孩童創意行動挑戰總監、印度河濱學校校長吉蘭‧貝兒‧瑟吉(Kiran Bir Sethi)認為，傳統教育並不是將學習的焦點放在理解與學習，而是把焦點放在記憶與研讀，孩子到學校學習不是因為他們有求知的欲望，而是為了考試。</p>
      <p><br></p>
      <p>吉蘭‧貝兒‧瑟吉說，若是沒有學習解決生活問題的能力，面對未來，這樣的學習系統已經不再有功用。共玩創作總監吳彥杰說，「現在已經不是大量製造完成，他就可以進入到職場發揮作用的時代了。」</p>
      <p><br></p>
      <p><br></p>
      <h3 class="subtitle">孩子，你可以不乖</h3>
      <p><br></p>
      <p>從小到大，我們被要求乖乖的，乖乖吃飯、乖乖聽話、乖乖上課，得要按照社會的主流價值長大才算乖。</p>
      <p><br></p>
      <p>成功大學資訊工程系教授蘇文鈺從小六開始拿烙鐵學著焊電路，因為「不太乖」找到了一生的興趣與志業，他觀察，現代的孩子失去了不乖的機會，如果太乖就很難作怪，害怕接觸新事物、也害怕失敗。</p>
      <p><br></p>
      <p>吳彥杰說，亞洲國家的教育普遍養成過度服從的孩子，最知名的例子是，韓國世越號沉沒，許多孩子聽船長的話躲在櫃子裡，活活被淹死。只有極少數的孩子想說要不要出去看一看，這些是韓國社會中認為不聽話的孩子，卻成了少數活命的孩子。</p>
      <p><br></p>
      <p>吉蘭‧貝兒‧瑟吉認為，學習應該要讓孩子不侷限在書桌前，而是真正的練習選擇、合作與想像力，在旁協助引導的大人，也能相信孩子的選擇，而學習的知識應該要可以應用在生活中，這才是學習應有的樣貌。</p>
      <p><br></p>
    </content-container>
    <animation-image style="background-color: black" :animationConfig1="srcRWD(imgMob1, imgWeb1)" aniamtionRef1="image1"  >
      <template slot="describe">
        <p style="color: gray">成功大學資訊工程系教授蘇文鈺認為，傳統教育有許多框架，讓孩子無法享受學習的樂趣。圖／蘇文鈺提供</p>
      </template>
    </animation-image>
    <content-container  style="background-color: black; color: white">
      <p><br></p>
      <p><br></p>
      <h3 class="subtitle">為什麼不問問題？</h3>
      <p><br></p>
      <p>蘇文鈺說，他常帶學生到國外比賽，台灣技術並不輸人，但就是不太會講，他看到國外團隊，明明做的東西也沒什麼，卻講得天花亂墜，「台灣人不會表達自己，會是與國際競爭的弱點」。</p>
      <p><br></p>
      <p>為什麼吝於表達自己？DFC全球孩童創意行動挑戰台灣發起人許芯瑋認為，這是因為從小到大孩子接收到的訊息是「你長大再說」，小時候孩子想做的天馬行空想法，大人會告訴你「等你高一點、強壯一點、甚至有錢了再說」，現在只要乖乖念書什麼都不用想。<span class="highlight">因為被壓抑慣了，所以有什麼想法好像說出來也沒有用。</span></p>
      <p><br></p>
      <p>吳彥杰教孩子拍動畫，一支動畫可以學習劇本的寫作、分鏡鏡頭、顏色搭配，但對孩子而言，最難的部分仍是寫劇本，孩子普遍不會自我表達，而這反而是面對未來最急需的能力。</p>
      <p><br></p>
      <p><br></p>
      <h3 class="subtitle">弄丟了好奇心</h3>
      <p><br></p>
      <p>明明國小的教學現場，小學生總是機哩瓜啦永遠都有一百個為什麼，為什麼孩子長大了，卻反而越來越沉默？對這個世界的熱情，隨著年齡增長而逐年下降？</p>
      <p><br></p>
      <p>「台灣的教育是一個框架，沒有太多彈性」，蘇文鈺說，過去他國中三年，前兩年有很多空白時間看課外書、鑽研有興趣的領域，最後好好念一年衝刺聯考，有一些空白時間可以運用。</p>
      <p><br></p>
      <p>蘇文鈺認為，現在教育的框架越縮越緊，分數是框架，現在還要求要做多少時數的志工，參加多少比賽換點數，入學管道看似多元，但最後還是在看分數，無法享受學習的樂趣。</p>
      <p><br></p>
      <p>「傳統教育孩子最缺乏的就是學習的胃口與好奇心」吳彥杰認為，家長太周到了，拚命餵食孩子知識，就像每天吃buffet吃到撐，孩子對學習沒有欲望。在未來可能是必須創造第二、第三事業才能永續工作的世代，<span class="highlight">因此可能4、50歲還需要重新學習，「沒有好奇心是面對未來最危險的事情。」</span></p>
      <p><br></p>
    </content-container>
    <animation-image :animationConfig1="srcRWD(imgMob2, imgWeb2)" aniamtionRef1="image2" ></animation-image>
    <content-container>
      <anchor title="跳出生產線">
        <div class="main-title">
          <h3 class="title">他帶孩子跳出生產線</h3>
          <ul>
            <li class="green-line"></li>
            <li class="red-line"></li>
            <li class="black-line"></li>
            <li class="light-green-line"></li>
          </ul>
        </div>
      </anchor>
      <p><br></p>
      <p>現在的社會，反映的是20年前的教育。</p>
      <p><br></p>
      <p>越來越多教育工作者，看見傳統教育的不足，運用許多創新的教育方法教學，他們相信，唯有孩子長好了，社會才有可能走向共好。</p>
      <p><br></p>
      <p><br></p>
      <h3 class="subtitle2">創新教育不再是都市才藝班專利</h3>
      <p><br></p>
      <p>教育需要成本，若是創新教育建立在高成本上，就會加劇教育不平等、階級世襲。共玩創作總監吳彥杰認為視覺傳達教育不是都市才藝班的專利，他將教具成本壓低在200元，並深入鄉鎮教學，「不分貧富，孩子都能用視覺為自己說一個好故事」。</p>
      <p><br></p>
      <p>共玩創作為一個偶動畫團隊，以逐格動畫教孩子運用科技表達自我，吳彥杰說，視覺是最有效率的傳達語法，一張照片可能比一場演講更吸睛，<span class="highlight">未來孩子必須要用最爭取眼球的方式來傳達自我，才能在大量資訊變動的時代受注目、產生影響力。</span></p>
      <p><br></p>
      <p>吳彥杰說，現在的影視教育大多在大學裡學，許多孩子在小學3、4年級已開始接觸手機與平板，何不在他開始認識媒體時，扎下視覺教育的根？</p>
      <p><br></p>
      <p>一般人對動畫教育的印象，總認為是都市孩子才藝班的產物，吳彥杰不諱言，教育創新需要考慮到教學效率，例如一對一的家教比一對三的效率還好，帶孩子去環遊世界比關在教室裡上地理課效率還好，<span class="highlight">當教育創新需要建立在高成本上，就變成高效率教育只能建立在能負擔的人身上。</span></p>
      <p><br></p>
      <p>吳彥杰不願讓視覺教育有接觸的城鄉差距，他獲永齡教育基金會支持，走入鄉鎮教學，當他走進鄉下教室時，他看見孩子臉上總是寫著害怕失敗、擔心學不會，就連鄉下的老師也跟他說，「老師我跟你講，先給你打個預防針，孩子可能學得比較慢…」。</p>
      <p><br></p>
      <p>其實在相同的教材與時間下，鄉下孩子的作品並不亞於都市孩子，甚至更出色，吳彥杰說「偏鄉的孩子可能學習學科會比較慢，但學習視覺傳達沒有比較慢」。</p>
      <p><br></p>
      <p>吳彥杰認為，偏鄉孩子給他們上課的回饋是最好的，可是他們也是最早放棄的，因為課堂上教的知識跟他的未來沒有連結，還沒畢業就到工廠上班、去農田噴農藥，</p>
      <p><br></p>
      <p>「我們要啟發個人對未來的想像、家長對未來的想像」吳彥杰認為，對未來若有想像，才有求知的動力，教育工作者應該思考教孩子怎麼學，可以發揮他的能力。</p>
      </content-container>
    <animation-image :animationConfig1="srcRWD(imgMob3, imgWeb3)" aniamtionRef1="image3" >
      <template slot="describe">
        <p>共玩創作總監吳彥杰（右）讓視覺傳達教育深入鄉鎮，不再是都市才藝班的權利。記者蘇健忠／攝影</p>
      </template>
    </animation-image>
    <content-container>
      <p><br></p>
      <p><br></p>
      <h3 class="subtitle2">用程式、創客幫孩子找未來</h3>
      <p><br></p>
      <p>成功大學資訊工程系教授蘇文鈺創立中華民國愛自造者學習協會，在台南教導家庭支持系統薄弱的孩子寫程式、玩創客、飛空拍機，將孩子留在課堂上，為他們找未來，並帶領孩子看見家鄉的不足，未來若有能力，有機會改善家鄉成樂土。</p>
      <p><br></p>
      <p>蘇文鈺說，過去在偏鄉許多營隊、企業來來去去，孩子並不信任他們，直到他的團隊陪伴至第5年，「他們終於相信我們不會走了」，他們教孩子寫程式用的電腦甚至是6、7年前的再生電腦，但長期陪伴，給了孩子很大的安定力量。</p>
      <p><br></p>
      <p>5年的陪伴，可以改變什麼？蘇文鈺說，他最近引薦一個高中的學生到企業實習，行前他叮嚀，「以前我都不罵你們，如果在企業實習被罵，要知道自己錯在哪裡」，這名孩子懂事的說，「教授，你以前不罵我們是不必要的，<span class="highlight">我們做不好就該罵，我不會因為你罵我就不繼續學習，因為學習是我自己的事情</span>」。</p>
      <p><br></p>
      <p>蘇文鈺聽了，感動得說不出話來，很難想像5年前這個孩子，他對外界的關心愛理不理，遇到困難只想躲起來，他會說出這句話，代表他雖然仍受原生家庭的影響，但長大了、想法變得正面了。</p>
      <p><br></p>
      <p>除了替孩子找未來，蘇文鈺也提供獎學金，讓早期跟著他學程式的大孩子，回到他們的家鄉教更小的小孩，他也辦看見家鄉計畫，讓孩子用空拍機紀錄家鄉，孩子用心去看自己的家鄉的故事，「好的地方，將它保留下來，不好的地方，長大後要能夠改進它」。</p>
      <p><br></p>
      <p><span class="highlight">蘇文鈺眼中的創新教育「不是技術與硬體上的進步，而是如何時時刻刻為孩子的學習想出新的辦法。」</span></p>
    </content-container>
    <animation-image :animationConfig1="srcRWD(imgMob4, imgWeb4)" aniamtionRef1="image4" >
      <template slot="describe">
         <p>成功大學資訊工程系教授蘇文鈺教家庭支持系統薄弱的孩子寫程式，為孩子找未來。圖／蘇文鈺提供</p>
      </template>
    </animation-image>
    <content-container>
      <p><br></p>
      <p><br></p>
      <h3 class="subtitle2">知識除了用在考卷上　還有別的用處</h3>
      <p><br></p>
      <p>大人總愛跟孩子說「你長大再說」，全球孩童創意行動挑戰（Design For Change-DFC）台灣發起人許芯瑋相信孩子有解決問題的能力，運用「感受」、「想像」、「實踐」、「分享」4個設計思考步驟，讓孩子學習的知識化為實際行動，解決生活周遭的大小問題。</p>
      <p><br></p>
      <p>「孩子在學習的過程中，終於有地方運用所學」許芯瑋說，之前我們運用所學的地方都是在考卷裡，考完就還給老師，<span class="highlight">孩子在實踐DFC的過程中明白，真的能運用課堂上學的書寫與統計的能力去解決問題，他們就會書到用時方恨少。</span></p>
      <p><br></p>
    </content-container>
      <animation-image :animationConfig1="srcRWD(imgMob5, imgWeb5)" aniamtionRef1="image5" >
          <template slot="describe">
          <p>全球孩童創意行動挑戰台灣發起人許芯瑋運用設計思考步驟，相信孩子有解決問題的能力。記者王騰毅／攝影</p>
        </template>
      </animation-image>
     <content-container>
      <p><br></p>
      <p><br></p>
      <p>過去因為校園安全議題，有蓋圍牆或是拆圍牆的討論，許芯瑋舉例，台北市日新國小的孩子，「感受」到這個問題後，便思考如何不增加經費、保全的情況下，提升學生的安全感，他們找出校園裡的警鈴、逃生裝置，並設計闖關遊戲讓學生參與，也錄製影片教導其他學生遇到陌生人該如何應對。</p>
      <p><br></p>
      <p>另外的例子是，孩子發現爺爺奶奶不能吃自己的生日蛋糕，因為太油膩，他們就去找食譜，用代糖、豆漿、水果等較健康的食材，特製生日蛋糕，並到老人院陪爺爺奶奶一起吃蛋糕，許多老人家感動的拭淚「已經很久沒有人關心我了」，孩子發現他們的行動，真的可以幫助他人。</p>
      <p><br></p>
      <p>許芯瑋說，教學現場中常常會說「我幫你做的..」，<span class="highlight">這是Desigh for，有許多上對下、理所當然、腦補認為你需要學什麼，但何不試試Desigh  with，老師與孩子一起設計我們的教學現場，一起解決發現的問題。</span></p>
      <p><br></p>
      <p>許芯瑋說，當我們的老師不腦補了，真的透過對話了解學生的需求，以學生為中心，而不是以評分者為中心，以行政為中心的時候，不管是哪一種方式，就已經是教育創新了。</p>
      <p><br></p>
    </content-container>
    <animation-image :animationConfig1="srcRWD(imgMob7, imgWeb7)" aniamtionRef1="image7" >
        <template slot="describe">
          <p>LIS線上教學平台創辦人嚴天浩將國中小的自然課程，拍攝成趣味的科學影片，增加孩子的學習興趣。記者蘇健忠／攝影</p>
        </template>
    </animation-image>
    <content-container>
      <p><br></p>
      <p><br></p>
      <h3 class="subtitle2">面對未來　教材也要進化</h3>
      <p><br></p>
      <p>現代學生普遍對知識沒有欲望，LIS線上教學平台將國中小的自然課程以有趣的真人戲劇影片呈現，跳脫紙本，讓孩子看到科學家如何發現與解決問題，引發學習動機，這些科學教材讓老師、家長公益使用，全台約有六萬名學生使用，對科學更有感。</p>
      <p><br></p>
      <p>LIS線上教學平台的服務對象有偏鄉國中小的孩子、都市國中小的孩子、體制內的老師，他與台東孩子的書屋、永齡希望小學、無界塾合作，以影片討論自然課程，並實驗、實作，讓孩子思考並嘗試解決問題。</p>
      <p><br></p>
      <p>LIS線上教學平台創辦人嚴天浩說，無論菁英或弱勢，他在教學現場看到許多孩子缺乏自信、拒絕思考，當他拋出問題，孩子想都不想就說「你直接給我答案」，<span class="highlight">他們習慣了知識被準備好送至眼前，可是出了社會之後遇到的任何挑戰，沒有人為你送上答案。</span></p>
      <p><br></p>
      <p>「台灣教育喜歡用成績評價一個學生行或不行」，當嚴天浩用創新的方式帶領孩子接觸自然科學，他看到課堂中開始起了變化，過去不擅長考試的孩子，是主流價值中的邊緣人，但透過影片教學、實作後，因為「創造不同情境，讓原本的天賦得以發揮」，他成了班上最亮眼的孩子。</p>
      <p><br></p>
      <p>「如果把考卷從教學現場中拿開，老師有辦法跟學生說應該學什麼呢？」嚴天浩的夢想很大，希望將LIS線上教學平台的教材從體制外逐漸推廣到體制內，影響更多老師，已經有越來越多老師口耳相傳，將LIS的教材推薦給其他老師使用。</p>
      <p><br></p>
      <p>嚴天浩希望孩子最終相信自己學得會、願意接受挑戰，有勇氣與能力去做想做的事。</p>
    </content-container>
    <animation-image :animationConfig1="srcRWD(imgMob8, imgWeb8)" aniamtionRef1="image8" >
      <template slot="describe">
        <p>永齡教育基金會董事長郭守正認為，教育的核心精神應該引發孩子的學習動機，並讓孩子相信自己有解決問題的能力。記者余承翰／攝影</p>
      </template>
    </animation-image>
    <content-container>
      <p><br></p>
      <p><br></p>
      <h3 class="subtitle2">投資創新教育  比天使更佛心</h3>
      <p><br></p>
      <p>教育是深水區，走進來的人需要龐大資金與勇氣。</p>
      <p><br></p>
      <p>「台灣有很多年輕人努力著，我們也覺得他們沒有大的市場可以去實驗，來落實他們提出的方法，但這也是我們該扮演的角色，如何整合資源打造平台。」郭守正希望提供實驗與實踐的平台，不是由企業或基金會主導，而是讓更多年輕人參與。</p>
      <p><br></p>
      <p>郭守正強調，自己做的是拋磚引玉的事情，這個平台可以為孩子整合許多解決問題的工具與資源。他認為，幫孩子或年輕人排除障礙，正是企業與基金會應該做的事情。</p>
      <p><br></p>
      <p>永齡教育基金會執行長劉宥彤也表示，過去幾年永齡教育基金會支持的創新教育團隊，根據屬性不同，給予的資源協助就不相同。天使投資人評估「產品差異化」，也就是必須清楚這項教育產品「要解決教育哪個環節的問題」，目標受眾會是誰？</p>
      <p><br></p>
      <p>劉宥彤舉例，幫助偏鄉的孩子？還是適用所有家庭的孩子？比如永齡教育基金執行中的希望小學，只聚焦做「雙低」學童：學業低成就以及低社經家庭的孩子，這群學童欠缺的不只是學業上的幫助，他們很多人可能連洗個澡、可以換穿的乾淨內衣褲都欠缺，需要龐大的社工體系進入校園、家庭給予個案服務，已經超越一般補救教學層次了。</p>
      <p><br></p>
      <p>「企業家的本質，是為了解決社會問題。」劉宥彤也強調，<span class="highlight">創新教育是一場馬拉松，卻和企業的未來息息相關，會盡己所能為企業養才，也為社會養才。</span></p>
      <p><br></p>
      <p>「創新教育已經是一場社會運動，企業無法缺席。」劉宥彤強調，教育是點點滴滴的過程，不會有一夕之間的變化，但是未來世界的變化卻難以預測，未來將沒有單一成功模式，每一個社創或社企團隊，嘗試的都是可能的問題解方。</p>
      <p><br></p>
      <p><br></p>
      <share href="https://udn.com/upf/newmedia/2018_data/newedu/index.html"></share>
      <logo use-ubrand="yes" use-vision='no'>
        <div class="logo">
          <a href="http://www.yonglin.org.tw/" target="_blank"><img :src="logo"></a>
        </div>         
      </logo>
      <p><br></p>
      <editor>
        <div>製作人、文字：吳思萍</div>
        <div>網頁設計、影音製作：張心慈</div>
        <div>影音、攝影：蘇健忠、王騰毅、劉學聖、張心慈</div>
        <div>網頁製作：胡凈悟</div>
        <div>議題行銷：張乃文、陳欣媛、蔡嘉棋、王敏霏</div>
        <div>監製：林秀姿、董谷音、蔡幸怡、潘如瑩</div>
        <div>2018.12.25</div>
      </editor>
      <p><br></p>
      <relate title="延伸閱讀"
        text1="一起用設計改變世界 孩子也能成為倡議家" href1="https://ubrand.udn.com/ubrand/story/11817/3502497" :img1="related.read1"
        text2="早就是程式高手？開發App讓你免試進科大" href2="https://ubrand.udn.com/ubrand/story/11815/3503254" :img2="related.read2"
        text3="唐鳳：別教小孩當工具人 否則容易被AI取代" href3="https://ubrand.udn.com/ubrand/story/11815/3462557" :img3="related.read3"
        text4="身處科技時代 如何讓孩子發揮出人的天性？" href4="https://ubrand.udn.com/ubrand/story/11815/3475980" :img4="related.read4">
      </relate>
      <p><br></p>
      <fb-comment href="https://udn.com/upf/newmedia/2018_data/newedu/index.html"></fb-comment>
    </content-container>
    <back-top></back-top>
    <foot></foot>
  </div>
</template>

<script>
import Vue from 'vue'
import srcRWD from '@/mixin/srcRWD.js'
import AnimationCover from '@/components/AnimationCover.vue'
import AnimationImage from '@/components/AnimationImage.vue'
import globalComponents from '@/plugins/baseComponents.js'

Vue.use(globalComponents)

export default {
  name: 'App',
  mixins: [srcRWD],
  data () {
    return {
      logo: 'static/logo.jpg',
      quote: 'static/quote.png',
      eductionVideo: 'https://www.youtube.com/embed/tMKWb-5hQZA',
      related: {
        read1: 'static/related/read1-1.jpg',
        read2: 'static/related/read1-2.jpg',
        read3: 'static/related/read1-3.jpg',
        read4: 'static/related/read1-4.jpg'
      },
      coverWeb1: {
          renderer: 'svg',
          loop: true,
          autoplay: true,
          path: 'static/animation/cover/web/data.json'
      },
      coverMob1: {
          renderer: 'svg',
          loop: true,
          autoplay: true,
          path: 'static/animation/cover/mob/data.json'
      },
      imgWeb1: {
          renderer: 'svg',
          loop: true,
          autoplay: true,
          path: 'static/animation/image1/web/image1.json'
      },
      imgMob1: {
          renderer: 'svg',
          loop: true,
          autoplay: true,
          path: 'static/animation/image1/mob/data.json'
      },
      imgWeb2: {
          renderer: 'svg',
          loop: true,
          autoplay: true,
          path: 'static/animation/image2/web/image2_ex.json'
      },
      imgMob2: {
          renderer: 'svg',
          loop: true,
          autoplay: true,
          path: 'static/animation/image2/mob/image2_m.json'
      },
      imgWeb3: {
          renderer: 'svg',
          loop: true,
          autoplay: true,
          path: 'static/animation/image3/web/image3_ex.json'
      },
      imgMob3: {
          renderer: 'svg',
          loop: true,
          autoplay: true,
          path: 'static/animation/image3/mob/image3_m.json'
      },
      imgWeb4: {
          renderer: 'svg',
          loop: true,
          autoplay: true,
          path: 'static/animation/image4/web/data.json'
      },
      imgMob4: {
          renderer: 'svg',
          loop: true,
          autoplay: true,
          path: 'static/animation/image4/mob/image4_m.json'
      },
      imgWeb5: {
          renderer: 'svg',
          loop: true,
          autoplay: true,
          path: 'static/animation/image5/web/data.json'
      },
      imgMob5: {
          renderer: 'svg',
          loop: true,
          autoplay: true,
          path: 'static/animation/image5/mob/image5_m.json'
      },
      imgWeb7: {
          renderer: 'svg',
          loop: true,
          autoplay: true,
          path: 'static/animation/image7/web/data.json'
      },
      imgMob7: {
          renderer: 'svg',
          loop: true,
          autoplay: true,
          path: 'static/animation/image7/mob/data.json'
      },
      imgWeb8: {
          renderer: 'svg',
          loop: true,
          autoplay: true,
          path: 'static/animation/image8/web/data.json'
      },
      imgMob8: {
          renderer: 'svg',
          loop: true,
          autoplay: true,
          path: 'static/animation/image8/mob/data.json'
      }
    }
  },
  components: {
    'animation-cover': AnimationCover,
    'animation-image': AnimationImage
  },
  mounted () {}
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
    .coverTitle1 {
      @media screen and (min-width: 768px) and (max-width: 1023px) {
        margin-top: 25px;
        font-size: 45px;
      }
      @media screen and (min-width: 1024px) {
        margin-top: 25px;
        font-size: 45px;
      }
    }
    .coverTitle2 {
      @media screen and (min-width: 768px) and (max-width: 1023px) {
        margin-top: 0;
        font-size: 30px;
      }
      @media screen and (min-width: 1024px) {
        margin-top: 0;
        font-size: 30px;
      }
      
    }
    .main-title {
    position: relative;
    padding-bottom: 33px;
    color: black;
    ul {
      margin: 0;
      padding: 0;
      position: absolute;
      left: 0;
      bottom: 0;
      width: 50%;
      height: 6px;
      display: flex;
      list-style: none;
      .green-line {
        flex: 2;
        background-color: #2ca58d;
      }
      .red-line {
        flex: 2;
        background-color: #f46197;;
      }
      .black-line {
        flex: 4;
        background-color: #384156;
      }
      .light-green-line {
        flex: 5;
        background-color: #84bc9c;
      }
    }
  }
}
</style>
