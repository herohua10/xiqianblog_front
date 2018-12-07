<template>
    <div class="header-area row">
      <!--顶部导航栏-->
      <div id="site-nav" class="row">
        <div class="col-lg-12"></div>
      </div>
      <!--菜单导航栏-->
      <div id="menu-nav" class="row">
        <!--标题、描述-->
        <div class="col-lg-2 col-lg-offset-1" style="height: inherit;">
          <h3><strong>{{title}}</strong></h3>
          <p><i>{{desc}}</i></p>
        </div>
        <!--导航菜单-->
        <div class="col-lg-5" style="height: inherit">
          <ul class="nav nav-pills">
            <li><a href="#">首页</a></li>
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
        <div class="col-lg-3" style="height: inherit">
            <div class="input-group" style="position:absolute;left:0;top: 0;bottom: 0;right: 0;margin: auto">
              <input type="text" class="form-control" placeholder="搜你想搜...">
              <span class="input-group-btn">
              <button class="btn btn-default" type="button">
                 <span class="glyphicon glyphicon-search"></span>
              </button></span>
            </div>
        </div>
      </div>
    </div>
</template>

<script>
export default {
  name: 'HomeHeader',
  data () {
    return {
      title: '洗钱博客',
      desc: '记录点滴，感动常在'
    }
  }
}
</script>

<style scoped>
  #site-nav {
    height: 30px;
    background-color: #F4F7F8
  }
  #menu-nav {
    background-color: #ffffff;
    height: 90px;
    border-top: 1px solid #ddd;
    border-bottom: 1px solid #ddd;
    box-shadow: 0 1px 1px rgba(0, 0, 0, 0.04);
  }

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
    margin-left: 0px;
  }
  .nav-pills > li > a {
    color: #000;
  }
  .nav-pills > li > a:hover {
    color: #fff;
    background-color: #666;
  }
  .nav-pills > li > a:active,
  .nav-pills > li > a:focus {
    color: #fff;
    background-color: #C40000;
  }
  .dropdown-menu {
    border-radius: 0px;
    margin: auto;
    padding: 0 0;
  }
  .dropdown-menu > li {

  }
  .dropdown-menu > li > a {
    height: 40px;
    line-height: 40px;
    text-align: center;
  }
  .dropdown-menu > li > a:hover {
    background-color: #a9a9a9;
  }
  .divider {
    margin: auto;
  }
</style>
