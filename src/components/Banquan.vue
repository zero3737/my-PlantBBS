<template>
    <footer>
        <p>Copyright&nbsp;&nbsp;2019-7-5&nbsp;&nbsp;By&nbsp;&nbsp;莫恋晨兮</p>
    </footer>
</template>

<script>
export default {

   name: '',
   data() {

       return { }

   }
}
</script>

<style scoped lang="less">
    footer {

        background: url(http://demo.cssmoban.com/cssthemes6/cpts_1782_cqu/img/slider_2.jpg) no-repeat fixed;
        height: 100px;
        position: relative;
        display: flex;
        justify-content: center;
        align-items: center;
        color: @white;
        font-size: 16px;
        border-radius: 5px;

        &::after {

            content: "";
            display: block;
            background-color: rgba(0, 0, 0, .4);
            position: absolute;
            top: 0;
            bottom: 0;
            right: 0;
            left: 0;
            border-radius: 5px;

        }

    }
</style>