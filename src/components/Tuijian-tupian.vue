<template>
    <div class="tupian wow bounceInDown" :data-wow-delay="delay+'s'">
        <div class="biankuang">
            <div class="div-img">
                <img src="../assets/baihe.jpg" alt="" class="img-responsive">
                <div class="mengban">
                    <span class="glyphicon glyphicon-eye-open animated rollIn faster"></span>
                </div>
            </div>
        </div>
        <p><a>测试</a></p>
    </div>
</template>

<script>
export default {

   data() {

       return { }

   },
   props: ['delay'],
   mounted() {

        $(".biankuang").hover(function() {

           if( $(this).find(`span[class*="animated"]`).length < 1 ) {

                $(this).find(`span[class*="glyphicon glyphicon-eye-open"]`).addClass("animated");

           }

        });

   }
}
</script>

<style scoped lang="less">
    .tupian {

        .biankuang {

            border: 5px solid @gray-1;
            border-radius: 5px;
            transition: all 0.2s ease-out;
            box-shadow: 0px 0px 5px @gray;
            cursor: pointer;

            &:hover {

                transform: rotate(-3deg);
                box-shadow: 5px 5px 5px @white-1;
                position: relative;
                bottom: 3px;

                .mengban {

                    display: flex !important;

                }

                img {

                    filter: blur(3px);

                }

            }

            .div-img {

                overflow: hidden;
                margin: 5px;
                position: relative;

                img {

                    transition: all 0.2s ease-out;

                    &:hover {

                        transform: scale(1.25, 1.25);

                    }

                }

                .mengban {

                    position: absolute;
                    top: 0;
                    bottom: 0;
                    left: 0;
                    right: 0;
                    background-color: rgba(0, 0, 0, .3);
                    display: none;
                    justify-content: center;
                    align-items: center;


                    span[class*="glyphicon glyphicon-eye-open"] {

                        color: @white-1;
                        font-size: 24px;

                    }

                }

            }

        }

        p {

            margin: 10px 0px;
            text-align: center;
            font-weight: bold;

        }

    }

</style>