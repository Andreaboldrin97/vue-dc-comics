<template>
    <div class="col-8 mt-3 position-relative container-hero">
        <a :href="link">
            <img class="img-fluid" :src="imgUrl" :alt="title">
        </a>
        <div class="position-absolute bottom-0 start-0 ps-5 pb-3 fs-5 fw-bold text-white">{{ title }}</div>
    </div>
</template>

<script>
export default {
     props: {
        title: String,
        link: String,
        imgUrl: String,
  },
}

</script>

<style lang="scss" scoped>
img{
    width: 100%;
}


</style>