<template>
    <div class="col-4 bg-light ms-5 mb-3" style="width: 18rem;">
        <div>
            <img :src="imgUrl" class="card-img-top" :alt="title">
        </div>
        <div class="card-body">
            <h6><a :href="link">{{ title }}</a></h6>
            <p class="card-text">{{ text }}</p>
        </div>
    </div>
</template>

<script>
export default {
      props: {
        title: String,
        link: String,
        imgUrl: String,
        text: String
  },
}
</script>

<style lang="scss" scoped>
h6{
    a{
        color: black;
        text-decoration: none;
    }
}

</style>