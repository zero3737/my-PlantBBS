<template>
   <section class="">
        <div class="container">
            <div class="row">
                <div class="col-md-4" v-for="count in 3" :key="count">
                    <Neirong2Pankuai :delay='0.4+0.1*count'></Neirong2Pankuai>
                </div>
            </div>
        </div>
   </section>
</template>

<script>
import Neirong2Pankuai from "./Neirong-2-pankuai"

export default {

   data() {

       return { }

   },
    components: {

        Neirong2Pankuai

    }

}
</script>

<style scoped lang="less">

    section {

        margin: 15px 0px;

    }

</style>