<template>
    <v-container id="imgText"  class="d-flex" style="justify-content: center;" >
      <v-row>
        <v-col id="text"cols="12" md="6" style="color:  rgb(110, 110, 110) ;line-height: 50px">
     <h1>「経年を慈しむ」モノづくり。</h1>
      <p>木は木の、鉄は鉄の持つ素材感があり、<br>
      できるだけ自分でメンテナンスできる素材を選んでいます。<br>
      自身の良さを活かすため、過度な仕上げをせず、<br>
      オイルやワックスで自然な仕上がりにしていく。<br>
      <br>
      何かで塗り固めて一時的にきれいにみせるのではなく、<br>
      5年後10年後その素材が活かされているかをイメージしながら<br>
      それぞれの最終の仕上げを選択しています。<br>
      使い捨てではなく時には手を加えながら、<br>
      世代を超えて慈しめるものを作っていきたいと思います。<br></p>
      <v-btn style="margin-top: 10px;">
        上手工作所 WEBサイトはこちら
</v-btn>
      </v-col>
    <v-col id="img3"cols="12" md="6">
      <img src="https://jo-zu-works.site/img/pc/jozu_philosophy02.jpg" data-aos="fade-right" data-aos-easing="linear" data-aos-duration="2000" data-aos-offset="100" data-aos-delay="1000">
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

</style>
