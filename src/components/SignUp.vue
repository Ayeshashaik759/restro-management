<template>
  <img class="logo" src="../assets/restaurant_logo.png" />
  <h1>Sign UP</h1>
  <div class="register">
    <input type="text" placeholder="Enter Name" />
    <input type="text" placeholder="Enter Email" />
    <input type="Password" placeholder="Enter Password" />
    <button>Sign Up</button>
  </div>
</template>

<script>
export default {
  name: "SignUp",
};
</script>
<style>
.logo {
  width: 100px;
}

.register input {
  width: 300px;
  height: 40px;
  padding-left: 20px;
  display: block;
  margin-bottom: 30px;
  margin-left: auto;
  margin-right: auto;
  border: 1px solid #e07979;
}

.register button {
  width: 320px;
  height: 40px;
  border: 1px solid #e07979;
  color: #fff;
  background-color: #ffd044;
  cursor: pointer;
}
</style>
