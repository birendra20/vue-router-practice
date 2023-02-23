<template>
  <div class="Jobs">
    <h1>Job Page</h1>
    <div v-for="job in jobs" :key="job.id" class="job">
      <router-link :to="{ name: 'JobDetails', params: { id: job.id } }">
        <h2>{{ job.title }}</h2>
      </router-link>
    </div>
  </div>
</template>

<script>
export default {
  name: "Jobs",
  components: {},
  data() {
    return {
      jobs: [
        { title: "react developer", id: 1, details: "random text react" },
        { title: "vue developer", id: 1, details: "random text vue" },
        { title: "angular developer", id: 1, details: "random text angular" },
      ],
    };
  },
};
</script>

<style>
.job h2 {
  background: gainsboro;
  padding: 20px;
  border-radius: 10px;
  margin: 10px auto;
  max-width: 600px;
  cursor: pointer;
  color: rgba(65, 55, 54, 0.777);
}
.job h2:hover {
  background: whitesmoke;
}

.job a {
  text-decoration: none;
}
</style>
