<template>
  <div style="display: grid; grid-template-columns: 1fr 400px; height: 60px">
      <div style="margin-top: 20px; margin-left: 40px;">Welcome to R^2</div>
    <div class="links">
      <a>About</a>
      <a>Projects</a>
      <a>Contact Us</a>
    </div>
  </div>
</template>

<script>
export default {
  name: "Nav"
};
</script>

<style>
.links {
    display: flex;
    justify-content: space-around;
    margin-top: 20px;
}
</style>