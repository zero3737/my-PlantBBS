<template>
    <section>
        <div class="container">
            <div class="tuijian-header">
                <h4><span class="glyphicon glyphicon-map-marker"></span>小伙伴们正在看...</h4>
            </div>
            <div class="tuijian">
                <div>
                    <ul>
                        <li v-for="count in 6" :key="count">
                            <TuijianTupian :delay="0.1*count"></TuijianTupian>
                        </li>
                    </ul>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
import TuijianTupian from "./Tuijian-tupian"

export default {

   name: '',
   data() {

       return { }

   },
   components: {

       TuijianTupian

   }
}
</script>

<style scoped lang="less">

    .tuijian {

        overflow: auto;

    }
    .tuijian ul {

        display: flex;
        flex-wrap: wrap;
        justify-content: space-around;
        padding: 0px;

    }
    .tuijian ul li {

        margin: 0px 5px;
        margin-top: 5px;
        min-width: 150px;
        flex-basis: 170px;
        flex: 1;

    }

    @media screen and (min-width: 991px) and (max-width: 1200px) {

        .tuijian ul li {

            &:nth-last-child(1) {

                display: none;

            }

        }

    }

    @media screen and (min-width: 686px) and (max-width: 991px) {

        .tuijian ul li {

            &:nth-last-child(1),
            &:nth-last-child(2) {

                display: none;

            }

        }

    }

    .tuijian-header h4 {

        font-weight: bold;
        color: @blue;
        padding-bottom: 5px;
        border-bottom: 2px dashed @white-1;

    }

</style>