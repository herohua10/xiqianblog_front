<template>
    <div class="row header-area">
      <!--顶部导航栏-->
      <div class="row" style="height: 30px;background-color: #F4F7F8">
        <div class="col-lg-12"></div>
      </div>
      <!--菜单导航栏-->
      <div class="row" style="background-color: #ffffff">
        <!--标题、描述-->
        <div class="col-lg-1 col-lg-offset-2" style="height: inherit">
          <h3>洗钱博客</h3>
          <p>程序人生，永不止步</p>
        </div>
        <!--导航菜单-->
        <div class="col-lg-4 col-lg-offset-1" style="height: inherit">
          <ul class="nav nav-pills">
            <li class="active"><a href="#">首页</a></li>
            <li><a href="#">Java</a></li>
            <li><a href="#">MyBatis</a></li>
            <li><a href="#">算法</a></li>
            <li class="dropdown">
              <a class="dropdown-toggle" data-toggle="dropdown" href="#">
                Spring全家桶 <span class="caret"></span>
              </a>
              <ul class="dropdown-menu">
                <li><a href="#">SpringMvc</a></li>
                <li class="divider"></li>
                <li><a href="#">SpringBoot</a></li>
                <li class="divider"></li>
                <li><a href="#">SpringCloud</a></li>
                <li class="divider"></li>
                <li><a href="#">SpringSecurity</a></li>
              </ul>
            </li>
            <li><a href="#">其它</a></li>
          </ul>
        </div>
        <div class="col-lg-2 col-lg-offset-1" style="height: inherit;">
            <div class="input-group">
              <input type="text" class="form-control">
              <span class="input-group-btn">
              <button class="btn btn-default" type="button">
              搜索
              </button></span>
            </div><!-- /input-group -->
        </div>
      </div>
    </div>
</template>

<script>
export default {
  name: 'HomeHeader'
}
</script>

<style scoped>
  .nav-pills {

  }
  .nav-pills > li {
    float: left;
    text-align: center;
  }
  .nav-pills > li > a {
    border-radius: 0px;
    height: 90px;
    line-height: 80px;
    text-align: center;
  }
  .nav-pills > li + li {
    margin-left: 2px;
  }
  .nav-pills > li.active > a,
  .nav-pills > li.active > a:hover,
  .nav-pills > li.active > a:focus {
    color: #fff;
    background-color: red;
  }

</style>
