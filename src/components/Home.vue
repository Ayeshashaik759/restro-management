<template>
  <Header />
  <h1>Hello, {{ name }} welcome on home page</h1>
</template>

<script>
import Header from "./Header.vue";
export default {
  name: "Home",
  components: {
    Header,
  },
  data() {
    return {
      name: "",
    };
  },
  async mounted() {
    let user = localStorage.getItem("user-info");
    this.name = JSON.parse(user).name;
    if (!user) {
      this.$router.push({ name: "SignUp" });
    }
    let result = await axios.get("http://localhost:3000/restaurant");
    console.warn(result);
  },
};
</script>
