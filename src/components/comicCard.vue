<template>
    <div class="comic-container col-6 col-md-3 col-lg-2">
        <img :src="thumb" :alt="series">
        <h6 class="pt-2">{{ series }}</h6>
    </div>
</template>

<script>
export default {
    props: {
        thumb: String,
        price: String,
        series: String,
        type: String,
  },
}
</script>

<style lang="scss" scoped>
.comic-container{
    img{
        width: 150px;
        height: 150px;
        object-fit: cover;
        object-position: top;
    }
}
</style>