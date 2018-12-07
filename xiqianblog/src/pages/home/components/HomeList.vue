<template>
  <div>
    <div class="article" v-for="article of articleList" :key="article.id">
      <div class="coverArticleWrapper">
        <div class="title">
          <h4><strong>{{article.title}}</strong></h4>
        </div>
        <div class="summary">
          <p>
            {{article.summary}}
          </p>
        </div>
        <div class="releaseDate">
          <ul>
            <li>
              <span class="glyphicon glyphicon-calendar"></span>&nbsp;
              {{article.releaseDate}}
            </li>
            <li>
              <span class="glyphicon glyphicon-thumbs-up"></span>&nbsp;
              {{article.views}}
            </li>
            <li>
              <span class="glyphicon glyphicon-thumbs-up"></span>&nbsp;
              {{article.likes}}
            </li>
            <li>
              <span class="glyphicon glyphicon-calendar"></span>&nbsp;
              {{article.comments}}
            </li>
          </ul>
        </div>
      </div>
      <div class="coverImageWrapper">
          <img class="coverImage" :src="article.coverImage">
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'HomeList',
  props: {
    articleList: Array
  }
}
</script>

<style scoped>
  .article {
    background-color: #fff;
    border: 1px solid #ddd;
    box-shadow: 0 1px 1px rgba(0, 0, 0, 0.04);
    margin-top: 10px;
    overflow: hidden;
    width: 100%;
    height: 0;
    padding-bottom: 20%;
  }
  .coverImageWrapper {
    overflow: hidden;
    width: 30%;
    height: 0;
    padding-bottom: 20%;
    position: relative;
  }
  .coverImage {
    position: absolute;
    top:50%;
    left:50%;
    transform: translate(-50%,-50%);
  }
  .coverArticleWrapper {
    float: right;
    overflow: hidden;
    width: 70%;
    height: 0;
    padding-bottom: 20%;
  }
  .title {
    overflow: hidden;
    width: 100%;
    height: 0;
    padding-bottom: 8%;
    padding-left: 2%;
  }
  .summary {
    overflow: hidden;
    width: 100%;
    height: 0;
    padding-bottom: 15%;
    padding-left: 2%;
    padding-right: 2%;
  }
  .releaseDate {
    overflow: hidden;
    width: 100%;
    height: 0;
    padding-bottom: 5%;
    padding-left: 2%;
  }
  .releaseDate > ul {
    text-align: left;
  }
  .releaseDate > ul > li {
    float: left;
    list-style: none;
    margin-right: 2%;
  }
</style>
