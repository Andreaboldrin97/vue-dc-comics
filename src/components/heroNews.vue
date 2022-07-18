<template>
   <div class="row">
                  <div class="col-8 position-relative">
                      <a :href="link">
                           <img :src="imgUrl" :alt="title">
                      </a>
                      <div class="position-absolute bottom-0 start-0 ps-5 pb-3 fs-5 fw-bold text-white">{{ title }}</div>
                  </div>
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

<style>

</style>