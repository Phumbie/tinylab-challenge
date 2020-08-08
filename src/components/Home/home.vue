<template>
  <div>
    <Navbar />
    <div class="side">
      <Sidebar />
      <div class="main">
        <Main />
      </div>
    </div>
  </div>
</template>
<script>
import Sidebar from "../layouts/Sidebar";
import Navbar from "../layouts/Navbar";
import Main from "./main";
export default {
  components: {
    Sidebar,
    Navbar,
    Main,
  },
};
</script>
<style scoped>
.side {
  display: flex;
}
.main {
  width: 100%;
}
</style>