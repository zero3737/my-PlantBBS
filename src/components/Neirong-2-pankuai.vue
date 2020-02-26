<template>
   <div class="pankuai wow bounceInUp" :data-wow-delay="delay+'s'">
       <div>
           <h2><a>花毛茛</a></h2>
           <p>
                花毛茛（gèn），学名：Ranunculus asiaticus（L.）Lepech.，
                芹菜花，陆莲花，为毛茛科、花毛茛属多年生草本花卉。花色丰富，
                多为重瓣或半重瓣，花型似牡丹花，但较小，花直径一般为8cm~1ocm；
                叶似芹菜的叶，故常被称为芹菜花。原产于欧洲东南部和亚洲西南部。
                1596年英国人引入进行人工栽培，在园林和切花中很常见。现在各国多
                有栽培，荷兰、英国、法国、美国、日本等栽培较多，并且培育出许多
                切花和盆栽品种。中国在上世纪90年代开始从荷兰、日本等引种，作为
                切花、盆栽和春季花卉展览用花在个各大城市栽培有。
            </p>
       </div>
       <div>
           <ul>
               <li><span class="badge">-</span><a>测试</a></li>
               <li><span class="badge">-</span><a>测试</a></li>
               <li><span class="badge">-</span><a>测试</a></li>
               <li><span class="badge">-</span><a>测试</a></li>
               <li><span class="badge">-</span><a>测试</a></li>
               <li><span class="badge">-</span><a>测试</a></li>
               <li><span class="badge">-</span><a>{{delay}}</a></li>
           </ul>
       </div>
   </div>
</template>

<script>
export default {

   data() {

       return { }

   },
   props: ['delay']

}
</script>

<style scoped lang="less">
    .pankuai {

        margin: 15px 0px;
        border: 5px solid @green;
        border-radius: 10px;
        padding: 10px;
        transition: all 0.2s ease-out;

        &:hover {

            box-shadow: 5px 5px 5px @white-1;
            position: relative;
            bottom: 3px;

        }

    }
    .pankuai > div:first-child {

        background-color: @white-1;
        padding: 15px;
        border-radius: 5px;

    }
    .pankuai h2 {

        text-align: center;
        margin-top: 0px;

    }
    .pankuai p {

        overflow: hidden;
        display: -webkit-box;
        -webkit-box-orient: vertical;
        -webkit-line-clamp: 3;
        line-height: 25px;
        text-indent: 30px;
        max-height: 80px;

    }
    ul {

        padding: 0 15px;

    }
    ul li {

        border-bottom: 1px dashed @white-1;
        padding-bottom: 5px;
        margin: 10px 0;

    }
</style>