<template>
  <div>
    <h1>Jobs Details</h1>
    <p>The Job id is {{ id }}</p>
  </div>
</template>

<script>
export default {
  props: ["id"], //from router/index.js
  name: "JobDetails",
  //   data() {
  //     return {
  //       id: this.$route.params.id,
  //     };
  //   },
};
</script>

<style></style>
