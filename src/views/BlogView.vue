<template>
  <div class="oue-help">
    <h1>{{ PageName }}</h1>
    <p>{{ PageDesc }}</p>
    <div class="container">
      <div class="row">
        <div class="col-md-8">
          <div class="post-area">
            <BlogPost
              v-for="post in posts"
              :key="post.id"
              :title="post.title"
              :date="post.date"
              :content="post.content"
              :author="post.author"
              :category="post.category"
              :views="post.views"
            />
          </div>
        </div>
        <div class="col-md-4">
          <div class="sidebar">
            <BlogSidebar />
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import BlogPost from "@/components/Blog/BlogPost.vue";
import BlogSidebar from "@/components/Blog/BlogSidebar.vue";

import jsonposts from "../json/blog_posts.json";

export default {
  data: function () {
    return {
      PageName: "Blog",
      PageDesc: "This Is Blog Page",
      posts: jsonposts,
    };
  },
  name: "BlogView",
  components: {
    BlogPost,
    BlogSidebar,
  },
};
</script>
