<template>
  <nav class="nav">
    <p>african leadership university</p>
    <div class="nav-links">
      <a href="">home</a>
      <p>/</p>
      <a href="">mission</a>
      <p>/</p>
      <a href="">about</a>
    </div>
    <div class="nav-social-links">
      <a href="">ALU</a>
      <p>/</p>
      <a href="">instagram</a>
      <p>/</p>
      <a href="">youtube</a>
    </div>
  </nav>
</template>

<script>
export default {
  setup() {
    return {};
  },
};
</script>

<style lang="scss" scoped>
.nav {
  width: 100%;
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  position: sticky;
  padding: 1.2rem 3.2rem;
  background-color: rgb(0, 0, 0, 0.1);
  top: 0;
  p {
    font-size: 1.4rem;
    color: #1d2034;
    text-transform: uppercase;
  }

  .nav-links {
    display: flex;
    flex-direction: row;
    gap: 1.2rem;
    P,
    a {
      text-transform: uppercase;
      font-size: 1.4rem;
      color: #1d2034;
    }
  }

  .nav-social-links {
    display: flex;
    flex-direction: row;
    gap: 1.2rem;
    P,
    a {
      text-transform: uppercase;
      font-size: 1.4rem;
      color: #1d2034;
    }
  }
}
</style>
