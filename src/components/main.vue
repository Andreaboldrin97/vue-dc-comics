<template>
  <main class="bg-dark">
      <div class="text-white px-5 py-5">
          <h2>--> Content goes here <-- </h2>
      </div>
      <section>
        <div class="shopper d-flex p-5 text-white">
            <div class="pe-4">
                <img src="../assets/img/buy-comics-digital-comics.png" alt="">
                DIGITAL COMICS
            </div>
            <div class="pe-4">
                <img src="../assets/img/buy-comics-merchandise.png" alt="">
                DC MERCHANDISE
            </div>
            <div class="pe-4">
                <img src="../assets/img/buy-comics-shop-locator.png" alt="">
                COMIC SHOP LOCATOR
            </div>
            <div class="pe-4">
                <img src="../assets/img/buy-comics-subscriptions.png" alt="">
                SUBSCRIPTIONS
            </div>
            <div class="pe-4">
                <img src="../assets/img/buy-dc-power-visa.svg" alt="">
                DC POWER VISA
            </div>
      </div>
      </section>
  </main>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
@import "../styles/variables.scss";
.shopper{
    background-color: $colorBreand;
    img{
        width: 80px;
        height: 80px;
        object-fit: contain;

    }
}
</style>