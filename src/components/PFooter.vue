
<script>
</script>

<template>
    <div class="footer">
        <div>
            <ul class="list">
                <li class="title">DC COMICS</li>
                <li>Characters</li>
                <li>Comics</li>
                <li>Movies</li>
                <li>TV</li>
                <li>Games</li>
                <li>Videos</li>
                <li>News</li>
            </ul>
        </div>
        <div>
            <ul class="list">
                <li class="title">DC</li>
                <li>Terms Of Use</li>
                <li>Privacy policy (New)</li>
                <li>Ad Choices</li>
                <li>Advertising</li>
                <li>Jobs</li>
                <li>Subscriptions</li>
                <li>Talent Workshops</li>
                <li>CPSC Certificates</li>
                <li>Ratings</li>
                <li>Shop Help</li>
                <li>Contact Us</li>
            </ul> 
        </div> 
        <div>
            <ul class="list">
                <li class="title">SITES</li>
                <li>DC</li>
                <li>MAD Magazine</li>
                <li>DC Kids</li>
                <li>DC Universe</li>
                <li>DC Power Visa</li>
            
            </ul>
            <ul class="list">
                <li class="title">SHOP</li>
                <li>Shop DC</li>
                <li>Shop DC Collectibles</li>
            </ul>  
        </div>
    </div>
    <div class="bar-footer"></div>
    
</template>

<style lang="scss" scoped>
@use './../assets/styles/partials/variables' as *;

.footer{
    background-image: url(../assets/img/footer-bg.jpg);
    height: 400px;
    display: flex;
    gap: 2rem;
    
}

.list{
    @include list-footer
}

.title{
    @include title
}
</style>
