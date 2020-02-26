<template>
  <header class="denglu hidden-xs hidden-sm">
    <div class="container">
      <div class="row">
        <div class="col-md-4">
          <div class="touxiang">
              <div class="div-img">
                <a data-toggle="popover" data-placement="left" data-content="今天也要努力呢~" role="button" tabindex="0" data-trigger="focus">
                  <img src="../assets/touxiang.jpg" alt="" height="40px">
                </a>
              </div>
              <span>莫恋晨兮</span>
          </div>
        </div>
        <div class="sousuo col-md-4">
          <form class="form-inline">
            <div class="form-group">
              <input type="email" class="form-control" id="exampleInputEmail2" placeholder="站内搜索">
            </div>
            <button type="submit" class="btn btn-success"><span class="glyphicon glyphicon-search"></span>搜索</button>
          </form>
        </div>
        <div class="btn-denglu col-md-4">
            <div>
                <button type="button" class="btn btn-info" data-toggle="modal" data-target="#zhuce">立即注册</button>
                <a class="btn btn-default" href="#" role="button"><span class="glyphicon glyphicon-user"></span>登录</a>
            </div>
        </div>
      </div>
    </div>
    <!-- 注册模态框 -->
    <div class="modal fade" id="zhuce" tabindex="-1" role="dialog" aria-labelledby="myModalLabel">
      <div class="modal-dialog" role="document">
        <div class="modal-content">
          <!-- 头部 -->
          <div class="modal-header">
            <button type="button" class="close" data-dismiss="modal" aria-label="Close"><span aria-hidden="true">&times;</span></button>
            <h4 class="modal-title" id="myModalLabel">注册信息</h4>
          </div>
          <!-- 内容 -->
          <div class="modal-body">
            <form>
              <div class="form-group">
                <label for="exampleInputEmail1">用户名</label>
                <input type="email" class="form-control" id="exampleInputEmail1" placeholder="请输入用户名">
              </div>
              <div class="form-group">
                <label for="exampleInputPassword1">密码</label>
                <input type="password" class="form-control" id="exampleInputPassword1" placeholder="请输入密码">
              </div>
              <button type="submit" class="btn btn-default" style="display: none;">提交</button>
            </form>
          </div>
          <!-- 尾部 -->
          <div class="modal-footer">
            <button type="button" class="btn btn-default" data-dismiss="modal">返回</button>
            <button type="button" class="btn btn-primary">提交</button>
          </div>
        </div>
      </div>
    </div>
  </header>
</template>

<script>
export default {

  beforeCreate() {

    $(function () {

      $('[data-toggle="popover"]').popover();

    })

  }

}
</script>

<style scoped lang="less">

/* header */
.denglu {

  .sousuo,
  .btn-denglu {

    height: 50px;
    display: flex;
    align-items: center;
    justify-content: flex-end;

  }

}

span[class="glyphicon glyphicon-search"], 
span[class="glyphicon glyphicon-user"] {

  margin-right: 3px;
  vertical-align: -1px;

}

.touxiang {

  height: 50px;
  display: flex;
  align-items: center;

}

.div-img {

  border-radius: 20px;
  overflow: hidden;
  border: 1px solid @white-1;

  & + span {

    margin-left: 15px;
    font-size: 14px;

  }

}

a:focus {

  outline: none;

}

</style>
