<template>
  <div class="toast-parent">
    <div class="toast-div" v-bind:class="type">
      {{text}}
    </div>
  </div>
</template>

<script>
export default {
  name: "toast",
  props: ["text", "type"],
}
</script>

<style scoped>
div.toast-parent {
  display: flex;
  justify-content: flex-end;
  margin: 10px 0;
}

.toast-div {
  border: 1px solid whitesmoke;
  background: whitesmoke;
  padding: 5px 2px;
  color: #333333;
  width: 10%;
  border-radius: 5px;
  font-size: 18px;
  margin-right: 10px;
  position: relative;
  bottom: 80px;
  right: 20px;
}

.success {
  background: #8ae8a2;
  border: 1px solid #8ae8a2;
}

.info {
  background: whitesmoke;
  border: 1px solid whitesmoke;
}

.warn {
  background: #fff37a;
  border: 1px solid #fff37a;
}

.alert{
  border: 1px solid #ff6b6b;
  background: #ff6b6b;
}
</style>
