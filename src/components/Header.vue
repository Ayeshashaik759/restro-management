<template>
  <div class="nav">
    <router-link to="/">Home</router-link>
    <router-link to="add">Add Restaurant</router-link>
    <router-link to="update">Update Reataurant</router-link>
    <a v-on:click="logout" href="#">Logout</a>
  </div>
</template>
<script>
export default {
  name: "Header",
  methods: {
    logout() {
      localStorage.clear();
      this.$router.push({ name: "Login" });
    },
  },
};
</script>
<style>
.nav {
  background-color: #ffc004;
  overflow: hidden;
}
.nav a {
  float: left;
  color: #7f005f;
  text-align: center;
  padding: 10px 14px;
  text-decoration: none;
  font-size: 16px;
  margin-right: 4px;
}
.nav a:hover {
  background-color: #7f005f;
  color: #f1f1f1;
}
</style>
