<script>
import PCards from "./PCards.vue";

export default {
  data() {
    return {
      arrCards: [
        {
          thumb: "https://www.coverbrowser.com/image/action-comics/1-1.jpg",
          price: "$19.99",
          series: "Action Comics",
          type: "comic book",
        },
        {
          thumb:
            "https://www.panini.it/media/catalog/product/cache/a5b5dd3adfe0d321084804c738f29601/M/1/M1BLLA015ISBN_0.jpg",
          price: "$19.40",
          series: "American Vampire 1976",
          type: "comic book",
        },
        {
          thumb:
            "https://media.wired.com/photos/593384dad80dd005b42b2817/master/w_2560%2Cc_limit/Aquaman-16.jpg",
          price: "$20.00",
          series: "Aquaman",
          type: "graphic novel",
        },
        {
          thumb: "https://d29xot63vimef3.cloudfront.net/image/batgirl/1-1.jpg",
          price: "$0.90",
          series: "Batgirl",
          type: "comic book",
        },
        {
          thumb:
            "https://static.posters.cz/image/750/locandine-film-in-plexiglass-batman-prowl-comic-cover-i69653.jpg",
          price: "$5.99",
          series: "Batman",
          type: "comic book",
        },
        {
          thumb:
            "https://static.wikia.nocookie.net/marvel_dc/images/5/50/Batman_Beyond_v.1_1.jpg",
          price: "$3.40",
          series: "Batman Beyond",
          type: "comic book",
        },
        {
          thumb:
            "https://static.wikia.nocookie.net/marvel_dc/images/0/0d/Batman_Superman_Vol_1_1.jpg",
          price: "$1.50",
          series: "Batman/Superman",
          type: "comic book",
        },
        {
          thumb:
            "https://static.wikia.nocookie.net/marvel_dc/images/c/cf/Batman_Superman_Annual_Vol_2_1.jpg",
          price: "$5.00",
          series: "Batman/Superman Annual",
          type: "comic book",
        },
        {
          thumb:
            "https://static.wikia.nocookie.net/marvel_dc/images/5/54/Batman_The_Joker_War_Zone_Vol_1_1.jpg",
          price: "$5.99",
          series: "Batman: The Joker War Zone",
          type: "comic book",
        },
        {
          thumb:
            "https://static.wikia.nocookie.net/marvel_dc/images/6/64/Batman_Three_Jokers_Collected.jpg",
          price: "$6.99",
          series: "Batman: Three Jokers",
          type: "comic book",
        },
        {
          thumb:
            "https://static.wikia.nocookie.net/marvel_dc/images/f/f8/Batman_White_Knight_Presents_Harley_Quinn_Vol_1_1.jpg",
          price: "$11.50",
          series: "Batman: White Knight Presents: Harley Quinn",
          type: "comic book",
        },
        {
          thumb:
            "https://static.wikia.nocookie.net/marvel_dc/images/c/c8/Catwoman_Vol_2_1.jpg",
          price: "$22.22",
          series: "Catwoman",
          type: "graphic novel",
        },
      ],
    };
  },
  components: {
    PCards,
  },
};
</script>
<template>
    <div class="container-jumbo">
        <img class="img-jumbo" src="../assets/img/jumbotron.jpg" alt="">
    </div>
    <div class="black">
        <div class="main">
            <PCards
            v-for="card in arrCards"
            :key="card.series"
            :urlImg="card.thumb"
            :title="card.series"
            :price="card.price"
            />
        </div>
    </div>
    
  
    
    <div class="color-cont">
        <div class="max-container">
            <div class="bar-main">
                <div class="cont-img">
                    <img class="img-main" src="../assets/img/buy-comics-digital-comics.png" alt="">
                    <h5>DIGITAL COMICS</h5>
                </div>
                <div class="cont-img">
                    <img class="img-main" src="../assets/img/buy-comics-merchandise.png" alt="">
                    <h5>DC MERCHANDISE</h5>
                </div>
                <div class="cont-img">
                    <img class="img-main" src="../assets/img/buy-comics-subscriptions.png" alt="">
                    <h5>SUBSCRIPTION</h5>
                </div>
                <div class="cont-img">
                    <img class="img-main" src="../assets/img/buy-comics-shop-locator.png" alt="">
                    <h5>COMIC SHOP LOCATOR</h5>
                </div>
                <div class="cont-img">
                    <img class="img-main" src="../assets/img/buy-dc-power-visa.svg" alt="">
                    <h5>DC POWER VISA</h5>
                </div>
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
@use './../assets/styles/partials/variables' as *;

.container-jumbo {
    height: 500px;

}

.black{
    background-color: black;
}

.img-jumbo {
    width: 100%;
    height: 100%;
    background-size: cover
}


.color-cont {
    @include color-cont
}

.main {
    @include color-main;
}

.bar-main {
    @include mini-main;
}

.text {
    @include color-text-main;
}

.img-main {
    @include img-main;
}

.cont-img {
    @include container;
}
</style>
