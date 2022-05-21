<template>
  <div class="about">
    <h1>{{ PageName }}</h1>
    <p>{{ PageDesc }}</p>
  </div>
</template>

<script>
export default {
  data: function () {
    return {
      PageName: "About Us",
      PageDesc: "This Is Abute Us Page",
    };
  },
  name: "AboutView",
};
</script>
