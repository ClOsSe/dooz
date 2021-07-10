<template>
  <div>
    <div class="item">
      <p>
        {{ selected.value }}
      </p>
    </div>
  </div>
</template>
<script>
export default {
  props: ["selected"],
};
</script>
<style scoped>
.item {
  color: black;
  width: 288px;
  height: 282px;
  border: 5px solid rgb(53, 6, 141);
}
</style>
