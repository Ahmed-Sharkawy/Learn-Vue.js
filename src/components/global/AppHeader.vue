<template>
  <div class="header">
    <div class="container">
      <div class="logo">Ahmed AL Sharkawy</div>
      <ul>
        <router-link to="/" tag="li"><a>Home</a></router-link>
        <router-link to="/about" tag="li"><a>About</a></router-link>
        <router-link to="/help" tag="li"><a>Help</a></router-link>
        <router-link to="/blog" tag="li"><a>Blog</a></router-link>
      </ul>
    </div>
  </div>
</template>

<script>
export default {
  name: "AppHeader",
};
</script>

<style lang="scss" scoped>
.header {
  background-color: #333;
  color: #fff;
  overflow: hidden;

  .container {
    display: flex;
    justify-content: space-between;
    align-items: center;
  }
  .logo {
    font-size: 20px;
    padding: 10px;
  }

  ul {
    margin: 0;
    list-style: none;
    display: flex;
    justify-content: space-between;
    align-items: center;
    li {
      padding: 20px;
    }
    a {
      color: #fff;
      text-decoration: none;
    }
  }
}
</style>
