<template>
  <div class="post-box">
    <span class="post-views">{{ views }}</span>
    <h3 class="post-title">{{ title }}</h3>
    <span class="post-date">{{ date }}</span>
    <p class="post-content">{{ content }}</p>
    <div class="row">
      <div class="col-sm-6">
        <span class="post-author">{{ author }}</span>
      </div>
      <div class="col-sm-6 text-end">
        <span class="post-category">{{ category | uppercase }}</span>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  props: ["title", "date", "content", "author", "category", "views"],
  name: "BlogPost",
};
</script>

<style lang="scss" scoped>
.post-box {
  padding: 20px;
  background-color: #fff;
  box-shadow: 0 0 10px #ddd;
  position: relative;
  text-align: left;
  border-radius: 5px;
  margin-bottom: 20px;

  .post-views {
    position: absolute;
    top: 5px;
    right: 5px;
    background-color: #4caf50;
    padding: 1px 5px;
    color: #fff;
    text-align: center;
    font-weight: bold;
  }

  .post-title {
    font-weight: bold;
    color: #818080;
  }

  .post-date {
    display: block;
    padding: 0 0 5px;
    color: #888;
  }

  .post-content {
    line-height: 1.8;
    color: #666;
  }

  .post-author {
    background-color: #607d8b;
    padding: 6px 10px;
    border-radius: 5px;
    color: #fff;
  }

  .post-category {
    background-color: #1e8b58;
    padding: 6px 10px;
    border-radius: 5px;
    color: #fff;
  }
}
</style>
