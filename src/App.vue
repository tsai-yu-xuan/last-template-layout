<template>
  <v-app>
    <v-container fluid class="d-flex">
      <!-- 左側導航欄 -->
      <v-navigation-drawer style="width:8%; position: fixed; top: 0px; left: 330px; height: 100%; padding-top: 25px; background: rgb(223, 223, 222);">
        <v-list>
          <v-list-item>
            <img src="https://jo-zu-works.site/img/logo2.png">
          </v-list-item>
          <v-list-item>
            <v-btn class="no-shadow" style="background: none;"><a href="#" >Top</a></v-btn>
          </v-list-item>
          <v-list-item>
            <v-btn class="no-shadow" style="background: none;"><a href="#" >shop</a></v-btn>
          </v-list-item>
          <v-list-item>
            <v-btn class="no-shadow" style="background: none;"><a href="#" >Photo</a></v-btn>
          </v-list-item>
          <v-list-item>
            <v-btn class="no-shadow" style="background: none;"><a href="#" >Sign</a></v-btn>
          </v-list-item>
          <v-list-item class="image-row">
            <a href=""><img src="https://cdn-icons-png.flaticon.com/128/1077/1077042.png"></a>
          </v-list-item>
        </v-list>
      </v-navigation-drawer>
      <!-- 主內容區域 -->
      <v-main class="custom-main" style="width: 70%" col="10" lg="8">
        <v-container>
          <carousel01></carousel01>
          <card></card>
          <imgText></imgText>
        </v-container>
      </v-main>
    </v-container>
    <v-footer class="footer" padless style="background:rgb(150, 150, 150);">
      <v-container>
        <v-row>
          <v-col class="text-center">
            <img src="https://jo-zu-works.site/img/logo.png" alt="" style="width: 200px;">
            <p>&copy; 上手工作所. All rights Reserved.</p>
            <v-icon>mdi-facebook</v-icon>
            <v-icon>mdi-twitter</v-icon>
            <v-icon>mdi-linkedin</v-icon>
            <v-icon>mdi-instagram</v-icon>
          </v-col>
        </v-row>
      </v-container>
    </v-footer>
</v-app>
</template>

<script>
import { onMounted, nextTick } from 'vue'
import carousel01 from '@/components/carousel01.vue'
import card from '@/components/card.vue'
import imgText from '@/components/imgText.vue'

export default {
  components: {
    carousel01,
    card,
    imgText
  },

}


</script>

<style>
body{
  background: rgb(223, 223, 222);
}

#app{
  width: 59%;
  height: 100vh;
  margin: auto;
}

.v-navigation-drawer{
  border: none !important;
  position: absolute;
}

.v-navigation-drawer__content  {
  width: 200px;
  background: rgb(223, 223, 222);
  padding-left: 20%;

}
.v-navigation-drawer__content a{
  color: black;
}

.v-application__wrap  {
  background: rgb(223, 223, 222);
}


.v-list-item__content img {
  width: 100%;
  overflow: hidden;
}
/* 改v-btn文字顏色 */
.v-btn__content a {
  color: rgb(110, 110, 110) !important;
  text-decoration: none;
}

/* 移除 v-btn 的所有陰影 */
.v-btn.no-shadow {
  box-shadow: none !important;
}

.v-btn.no-shadow:hover {
  box-shadow: none !important;
}

.v-btn.no-shadow:focus {
  box-shadow: none !important;
}

.v-btn.no-shadow:active {
  box-shadow: none !important;
}
.v-list-item--variant-text{
  font-size: 10px !important;
  /* text-align: start !important; */
}
/* 將 v-list-item 內的 img 橫排顯示 */
/* .image-row {
  display: flex;
  justify-content: space-between;
} */

.image-row img {
  width: 27%; /* 調整圖片的寬度以適應父容器 */
  margin: 3px;
}
/*  v-main 样式 */
.custom-main {
  padding: 0 !important; /* 移除默认的 padding */
  padding-left:10% !important; 
}

card{
  padding-top: 100px;
}


</style>