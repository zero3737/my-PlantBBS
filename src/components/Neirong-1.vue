<template>
    <section class="Neirong-1">
        <div class="container">
            <div class="row">
                <div class="col-md-3 wow bounceIn">
                    <div class="left-neirong-1">
                        <h4>
                            <span class="glyphicon glyphicon-star">
                            </span><span class="biaoti">植物新知</span>
                        </h4>
                        <div class="div-img">
                            <img src="~@/assets/baihe.jpg" alt="" width="100%" class="img-rounded img-responsive">
                        </div>
                        <div>
                            <ul>
                                <li><span class="badge">-</span><a>加载中...</a></li>
                            </ul>
                        </div>
                    </div>
                </div>
                <div class="col-md-6 wow bounceIn" data-wow-delay="0.1s">
                    <div class="center-neirong-1">
                        <div class="tuchu">
                            <h2>
                                <a>加载中...</a>
                            </h2>
                            <p>
                                加载中...
                            </p>
                        </div>
                        <div style="margin-top: 25px;" class="list">
                            <ul>
                                <li><span class="badge">-</span><a>测试</a></li>
                                <li><span class="badge">-</span><a>测试</a></li>
                            </ul>
                        </div>
                    </div>
                </div>
                <div class="col-md-3 wow bounceIn" data-wow-delay="0.2s">
                    <div class="right-neirong-1">
                        <div>
                            <h4>
                                <span class="glyphicon glyphicon-tint">
                                </span><span class="biaoti">相关信息</span>
                            </h4>
                        </div>
                        <div>
                            <ul>
                                <li><span class="badge">-</span><a>测试</a></li>
                            </ul>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
export default {

   name: 'Neirong-1',
   data() {

       return { }

   }
}
</script>

<style scoped lang="less">
.left-neirong-1, .center-neirong-1, .right-neirong-1 {

    border: 1px solid @white-1;
    border-radius: 5px;
    border-top: 3px solid @green;

}
.right-neirong-1 {

    border-top: 3px solid @blue;

}
.right-neirong-1 .badge {

    background-color: @blue;

}
.Neirong-1 h4 {

    border-bottom: 1px solid @white-1;
    padding-bottom: 5px;

}

.Neirong-1 h4 span[class="glyphicon glyphicon-star"], span[class="glyphicon glyphicon-tint"] {

    vertical-align: -2px;
    margin-right: 5px;
    color: @orange;

}

.Neirong-1 .container {

    margin-bottom: 15px;

}

span[class="glyphicon glyphicon-tint"] {

    color: @blue;

}

.left-neirong-1 div {

    margin-top: 20px;

}

.div-img {

    overflow: hidden;
    border-radius: 5px;
    margin: 5px;
    transform: rotate(-3deg);
    box-shadow: 0 0 5px;

}
img {

    width: 100%;
    transition: all 0.2s ease-out;

}
img:hover {

    transform: scale(1.25, 1.25);
    transition: all 0.2s ease-out;

}

@media screen and (max-width: 992px) {

    img {

        height: 400px;

    }

}

@media screen and (max-width: 768px) {

    img {

        height: 300px;

    }

}

ul {

    padding: 0 15px;

}
ul li {

  border-bottom: 1px dashed @white-1;
  padding-bottom: 5px;
  margin: 10px 0;

}

.Neirong-1 .left-neirong-1 ul li:first-child {

    border-bottom: 1px solid @white-1;
    padding-bottom: 10px;

}

.Neirong-1 .left-neirong-1 {

    padding: 15px;
    padding-top: 10px;

}
.center-neirong-1 .tuchu {

    background: url(https://i.zw3e.com/img/pc/zwt.gif) no-repeat;
    background-color: @white-1;
    padding: 15px;
    border-radius: 5px;
    margin-top: 15px;

}
.center-neirong-1 .tuchu p {

    display: -webkit-box;
    -webkit-box-orient: vertical;
    -webkit-line-clamp: 2;
    overflow: hidden;
    text-overflow: ellipsis;
    line-height: 25px;

}
.Neirong-1 .center-neirong-1 h2 {

    text-align: center;

}
.Neirong-1 .center-neirong-1 p {

    text-indent: 25px;

}
.row > div {

    margin: 15px 0;

}
.row > div > div {

    box-shadow: 5px 5px 5px @white-1;
    padding: 15px;

}
</style>