<template>
  <header class="container-fluid">
      <div class="d-flex p-3 justify-content-between">
          <div >
              <img class="logoBreand" src="../assets/img/dc-logo.png" alt="Main logo DC">
          </div>
          <nav>
            <ul class="d-flex justify-content-around">
                <li class="m-2" v-for="(link , index) in navLink" :key="index" >
                    <a :class="{active : link.active}" class="fw-bolder" :href="link.href" >{{ link.text }}</a>
                </li>
            </ul>
          </nav>
      </div>
  </header>
</template>

<script>
export default {
    data : function(){
    return {
      navLink : [
            {
                text : 'characters' ,
                href : '#',
                active : false
            },
            {
                text : 'comics' ,
                href : '#',
                active : true
            },
            {
                text : 'movies' ,
                href : '#',
                active : false
            },
            {
                text : 'tv' ,
                href : '#',
                active : false
            },
            {
                text : 'games' ,
                href : '#',
                active : false
            },
            {
                text : 'collectibles' ,
                href : '#',
                active : false
            },
            {
                text : 'videos' ,
                href : '#',
                active : false
            },
            {
                text : 'fans' ,
                href : '#',
                active : false
            },
            {
                text : 'news' ,
                href : '#',
                active : false
            },
            {
                text : 'shop' ,
                href : '#',
                active : false
            },

        ],
    }
}
}
</script>

<style lang="scss" scoped>
@import "../styles/variables.scss";
header{
    height: 100px;
    background-color: white;
}
.logoBreand{
    width: 70%;
    min-width: 70px;
    min-height: 70px;
}
nav{
    li{
        list-style: none;
        a{
             padding: 50px 0;
            text-decoration: none;
            color: $colorTextNav;
        }
    }
}
.active{
    color: $colorBreand;
    border-bottom: 5px solid $colorBreand ;
}

</style>