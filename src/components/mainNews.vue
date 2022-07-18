<template>
  <div>
      <div class="px-5 py-5">
          <h1>THE NEWS</h1>
          <div class="container-fluid mt-5">
              <div class="row">
                   <heroNews v-for="(news, index) in heroNews" :key="index"
                    :title="news.title"
                    :link="news.link"
                    :imgUrl="news.imgUrl"/>

                    <cardNews  v-for="(card, index) in cardsNews" :key="index"
                    :title="card.title"
                    :link="card.link"
                    :imgUrl="card.imgUrl"
                    :text="card.text"/>
                  

              </div>
          </div>
      </div>
  </div>
</template>

<script>
import heroNews from './heroNews.vue'
import cardNews from './cardNews.vue'

export default {
components: {
heroNews,
cardNews,

  },
  data: function(){
      return{
          heroNews : [{
                title : 'The Hero thst Supergirl Needs',
                link : 'https://www.dccomics.com/',
                imgUrl : 'https://www.dccomics.com/sites/default/files/styles/front_news_featured/public/field/image/SuperHereFor_BlogRoll_SCWOT_62d0f450cc2510.80215301.jpg?ito',
                
            }
          ],
          cardsNews :[
              {
                title : 'Super Work Friends: How the Justice League Gets Along',
                link : 'https://www.dccomics.com/blog/2022/07/14/super-work-friends-how-the-justice-league-gets-along',
                imgUrl : 'https://www.dccomics.com/sites/default/files/styles/front_news_default/public/field/image/BLOGroll2_SuperWorkFriends_62d0980d926e23.99167444.jpg?itok=UXIuae9a',
                text : "In Aquaman & The Flash: Voidsong, the Fastest Man Alive and the greatest hero of the seas team up against an alien invader that threatens all life on Earth. It’s not an..."
              },
              {
                title : "Batman '89 is a Delicious Dash of Dark Knight Nostalgia",
                link : 'https://www.dccomics.com/blog/2022/07/13/batman-89-is-a-delicious-dash-of-dark-knight-nostalgia',
                imgUrl : 'https://www.dccomics.com/sites/default/files/styles/front_news_default/public/field/image/Blogroll_GothamGazette_20220713_BM89_6_62ce34dee96065.40710917.jpg?itok=CokG5LJ8',
                text : "There’s something magical about the world of Tim Burton’s Batman. For an entire generation of fans, Michael Keaton was the Dark Knight. Batman and Batman Returns were comic..."
              },
              {
                title : 'V for Variety: Aqua-Horror, Swamp Things and Batman Opera with Ram V',
                link : 'https://www.dccomics.com/blog/2022/07/12/v-for-variety-aqua-horror-swamp-things-and-batman-opera-with-ram-v',
                imgUrl : 'https://www.dccomics.com/sites/default/files/styles/front_news_default/public/field/image/RamVInterview_blog_62ccdb783c8165.27357698.jpg?itok=vbud1adk',
                text : "Author of critically acclaimed and award-winning titles like These Savage Shores, Blue in Green and The Many Deaths of Laila Starr, DC’s history with Ram V started in 2018,..."
              },
              {
                title : 'Is Batman as Blind as a Bat?',
                link : 'https://www.dccomics.com/blog/2022/07/11/is-batman-as-blind-as-bat',
                imgUrl : 'https://www.dccomics.com/sites/default/files/styles/front_news_default/public/field/image/BATMAN%20125%20double-COVER_RGB_900_62c8e67d6f37d5.45154941.jpg?itok=zsJPP_Ah',
                text : "Batman might be the World’s Greatest Detective, but there are times when he misses the obvious. Batman #125 was published last week, kicking off a new creative era with..."
              },
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