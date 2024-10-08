<template>
  
<div id="text">
  <h1>Philosophy</h1>
  <p>上手工作所のモノづくり</p>
</div>

  <div id="img">
    <img src="https://jo-zu-works.site/img/pc/jozu_philosophy02.jpg" data-aos="fade-right" data-aos-easing="ease-out-cubic" data-aos-duration="2000" data-aos-offset="200" data-aos-delay="1000">
    <img src="https://jo-zu-works.site/img/pc/jozu_philosophy01.jpg" data-aos="fade-up-left" data-aos-easing="ease-out-quad" data-aos-duration="3000" data-aos-offset="100" data-aos-delay="2000">
  </div>

    <v-container style="margin-top: 100px;">
      <v-row>
        <v-col id="img2"cols="12" md="6">
          <img src="https://jo-zu-works.site/img/pc/jozu_philosophy03.jpg" data-aos="fade-right" data-aos-easing="ease-out-cubic" data-aos-duration="3000" data-aos-offset="200" data-aos-delay="000">
        </v-col>
        <v-col id="text2"cols="12" md="6" style="color:  rgb(110, 110, 110)">
          <h1>素材と向き合い、手を動かす。</h1>
          <p>「素材の魅力を最大限に引き出す」<br>
          わたしたちのものづくりの原点です。
          <br>
          <br>
          素材と向き合い、自分たちで考え、<br>
          ひとつひとつ手を動かし作る。<br>
          そして自らの手で販売し、お客様の元へ。<br>
          <br>
          木々が芽生えて育つ200年前の時から<br>
          ひとの暮らしに寄り添う50年先、100年先の未来まで想いを馳せて。<br>
          <br>
          「上手工作所」は豊かな自然に育まれた木々と<br>
          ひとの間を気持ちよく取り持って、ちょうどいいあんばいの暮らしの<br>
          エッセンスをお届けする、ものづくりのプロフェッショナルを目指しています。<br>
          </p>
        </v-col>
      </v-row>
    </v-container>
</template>

<script setup>
// 引入 AOS 动画库
import AOS from 'aos'
// 引入 AOS 动画库的 CSS 文件ss'
import 'aos/dist/aos.css'
// 初始化
AOS.init()
</script>

<style scoped lang="scss">

#text{
  margin: 100px;
  color: rgb(66, 66, 66);
  h1{
    font-size: 30px;
  }
  p{
    font-size: 12px;
    font-weight: bold;
  }
}

// #text2{
//   width: 400px;
//   position: relative;
//   top: -50px;
//   left: 450px;
//   color: rgb(66, 66, 66);
//   h1{
//     font-size: 25px;
//     padding-bottom: 10px;
//   }
//   p{
//     font-size: 12px;
//     // font-weight: bold;
//   }
// }

#img{
  display: flex;
  justify-content: start;
  img{
    
    &:nth-child(1){
      width: 240px;
      height: 320px;
      margin-top: 0px;
      left: 10px;
    }
    &:nth-child(2){
      width: 590px;
      height: 400px;
      margin-top: -130px;
      margin-left: 50px;
    }
  }
}
#img2{
  width: 200px;
  height: 200px;
  img{
    width: 80%;
    position: relative;
    left: 60px;
  }

}

#text2{
  width: 200px;
  height: 500px;
  position: relative;
  top: -80px;
}

</style>