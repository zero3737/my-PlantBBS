<template>
    <nav class="navbar navbar-default">
        <div class="container-fluid">
            <div class="navbar-header">
                <button type="button" class="navbar-toggle collapsed" data-toggle="collapse"
                        data-target="#bs-example-navbar-collapse-1" aria-expanded="false">
                    <span class="icon-bar"></span>
                    <span class="icon-bar"></span>
                    <span class="icon-bar"></span>
                </button>
                <a class="navbar-brand" href="#" style="color: #fff;">植物鉴赏</a>
            </div>

            <div class="collapse navbar-collapse" id="bs-example-navbar-collapse-1">
                <div class="div-ul">
                    <ul class="nav navbar-nav">
                        <li class=""><a href="#">春天与植物</a></li>
                        <li><a href="#">夏天与植物</a></li>
                        <li><a href="#">秋天与植物</a></li>
                        <li><a href="#">冬天与植物</a></li>
                    </ul>
                </div>
            </div>
        </div>
    </nav>
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
/* nav */
@s: @s1 ul;
@s1: ~".div-ul";

nav @{s1}, @{s} {

    display: flex;

}
@{s} {

    flex: 1;

    li {

        flex: 1;
        text-align: center;

    }

}


@media screen and (max-width: 768px) {

    nav @{s1}, @{s} {

        flex-direction: column;

    }
    nav a[class="navbar-brand"] {

        padding: 15px 30px;

    }

}

@media screen and (min-width: 768px) {

    nav a[class="navbar-brand"] {

        padding: 15px 60px;

    }

}

.navbar-default, nav .div-ul ._active a, nav .div-ul ._active a:hover {

    background-color: @green;
    color: @white;

}

/* 选中效果加载 nav 类里的 li 标签。 */
._active a, nav li:hover a {

    background-color: @green-1!important;
    border-radius: 5px;
    margin: 0 1px;

}

.navbar-default {

    .navbar-nav > li > a {

        font-weight: bolder;
        color: @white;

    }
    .navbar-toggle {

        &:focus, &:hover {

            background-color: @green-1 !important;

        }
        .icon-bar {

            background-color: @white;

        }

    }
    
}

</style>