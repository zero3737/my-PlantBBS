<template>
    <section>
        <div class="container wow bounceInRight" data-wow-delay="0.3s">
            <div>
                <div id="carousel-example-generic" class="carousel slide" data-ride="carousel">
                    <!-- Indicators -->
                    <ol class="carousel-indicators">
                        <li data-target="#carousel-example-generic" data-slide-to="0" class="active"></li>
                        <li data-target="#carousel-example-generic" data-slide-to="1"></li>
                        <li data-target="#carousel-example-generic" data-slide-to="2"></li>
                        <li data-target="#carousel-example-generic" data-slide-to="3"></li>
                    </ol>

                    <!-- Wrapper for slides -->
                    <div class="carousel-inner" role="listbox">
                        <div class="item active">
                            <div :style="{'background-image': `url(${require('../assets/1.png')})`}">
                            </div>
                        </div>
                        <div class="item"  v-for="count in 3" :key="count">
                            <div :style="{'background-image': `url(${require(`../assets/${count + 1}.png`)})`}">
                            </div>
                        </div>
                    </div>

                    <!-- Controls -->
                    <a class="left carousel-control" href="#carousel-example-generic" role="button" data-slide="prev">
                        <span class="glyphicon glyphicon-chevron-left" aria-hidden="true"></span>
                        <span class="sr-only">Previous</span>
                    </a>
                    <a class="right carousel-control" href="#carousel-example-generic" role="button" data-slide="next">
                        <span class="glyphicon glyphicon-chevron-right" aria-hidden="true"></span>
                        <span class="sr-only">Next</span>
                    </a>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
export default {

   name: '',
   data() {

       return {

       }

   }
}
</script>

<style scoped lang="less">

img {

    box-shadow: 0px 0px 0px;
    transform: rotate(0deg);

}
.item > div:first-child {

    height: 100px;
    background-size: cover;
    background-position: center center;
    background-repeat: no-repeat; 

}

.container > div {

    border-radius: 5px;
    box-shadow: 0px 0px 5px @black;
    overflow: hidden;

}

.carousel-indicators {

    bottom: 0px;

}

</style>