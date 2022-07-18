<template>
  <div>
      <div class="px-5 py-5">
          <h1>THE NEWS</h1>
          <div class="container-fluid mt-5">
             <heroNews v-for="(news, index) in heroNews" :key="index"
                    :title="news.title"
                    :link="news.link"
                    :imgUrl="news.imgUrl"/>
          </div>
      </div>
  </div>
</template>

<script>
import heroNews from './heroNews.vue'
export default {
components: {
heroNews,

  },
  data: function(){
      return{
          heroNews : [{
                title : 'The Hero thst Supergirl Needs',
                link : 'https://www.dccomics.com/',
                imgUrl : 'https://www.dccomics.com/sites/default/files/styles/front_news_featured/public/field/image/SuperHereFor_BlogRoll_SCWOT_62d0f450cc2510.80215301.jpg?ito',
            }
          ]
      }
  }
}
</script>

<style lang="scss" scoped>
@import "../styles/variables.scss";

h1{
    color: $colorBreand ;
}
</style>