<template>
  <div class="top">
    <div class="header_top">
      <div class="logo">
        <img
          src="../assets/logo.jpg"
          alt=""
        >
        <h1>智慧园区管理系统</h1>
      </div>
      <button
        v-if="flag"
        class="free"
        @click="goAbout"
      >免费使用</button>
    </div>
  </div>

</template>

<script>
export default {
  props: {
    flag: {
      type: Boolean,
      default: true,
    },
  },
  methods: {
    goAbout() {
      this.$router.push({ path: "/About" });
    },
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.top {
  background-color: #fff;
  .header_top {
    display: flex;
    align-items: center;
    justify-content: space-between;
    height: 100%;
    padding: 0 20px;
    .logo {
      display: flex;
      align-items: center;
      img {
        height: 60px;
      }
      h1 {
        margin-left: 10px;
      }
    }
    .free {
      border: 1px solid #289fee;
      color: #289fee;
      background-color: #fff;
      padding: 5px 10px;
      border-radius: 10px;
    }
  }
}
</style>
