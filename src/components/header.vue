<template>
  <header class="container-fluid">
      <div class="d-flex py-3 px-5 justify-content-between">
        <div>
            <img class="logoBreand" src="../assets/img/dc-logo.png" alt="Main logo DC">
        </div>
        <nav>
            <ul class="d-flex justify-content-around">
                <li class="m-2" v-for="(link , index) in navLinks" :key="index" >
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
      navLinks : [
            {
                text : 'CHARACTERS' ,
                href : '#',
                active : false
            },
            {
                text : 'COMICS' ,
                href : '#',
                active : true
            },
            {
                text : 'MOVIES' ,
                href : '#',
                active : false
            },
            {
                text : 'TV' ,
                href : '#',
                active : false
            },
            {
                text : 'GAMES' ,
                href : '#',
                active : false
            },
            {
                text : 'COLLECTIBLES' ,
                href : '#',
                active : false
            },
            {
                text : 'VIDEOS' ,
                href : '#',
                active : false
            },
            {
                text : 'FANS' ,
                href : '#',
                active : false
            },
            {
                text : 'NEWS' ,
                href : '#',
                active : false
            },
            {
                text : 'SHOP' ,
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
        &:hover{
            cursor: pointer;
        }
    }
}
.active{
    color: $colorBreand;
    border-bottom: 5px solid $colorBreand ;
}

</style>