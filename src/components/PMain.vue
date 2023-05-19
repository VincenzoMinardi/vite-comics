<script>
</script>

<template>
    <div class="main">
        <h2 class="text"> Content goes here</h2>
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

.color-cont{
    @include color-cont
}

.main{
    @include color-main;
}

.bar-main{
    @include mini-main;
}

.text{
    @include color-text-main;
}

.img-main{
    @include img-main;
}
.cont-img{
    @include container;
}

</style>
