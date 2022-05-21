<template>
  <div class="oue-help">
    <h1>{{ PageName }}</h1>
    <p>{{ PageDesc }}</p>
  </div>
</template>

<script>
export default {
  data: function () {
    return {
      PageName: "Help",
      PageDesc: "This Is Help Page",
    };
  },
  name: "HelpView",
};
</script>
