<template>
  <div>
    <p class="msg">{{msg}}</p>
  </div>
</template>

<script>
export default {
  data() {
    return {
      msg: "helloVue"
    };
  }
};
</script>
<style>
.msg {
  color: burlywood;
  font-size: 30px;
}
</style>