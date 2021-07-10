<template>
  <q-page class="flex flex-center">
    <div class="main-box">
      <ul class="node q-pa-none">
        <li
          class="row inline note-item q-ma-xs"
          v-for="(item, index) in NodeList"
          :key="index"
        >
          <SingleNote :selected="item" />
        </li>
      </ul>
    </div>
  </q-page>
</template>
<script>
import SingleNote from "../components/singlenode/SingleNode.vue";
export default {
  name: "PageIndex",
  data() {
    return {
      NodeList: [
        { value: "1", id: "1" },
        { value: "2", id: "2" },
        { value: "3", id: "3" },
        { value: "4", id: "4" },
        { value: "5", id: "5" },
        { value: "6", id: "6" },
        { value: "7", id: "7" },
        { value: "8", id: "8" },
        { value: "9", id: "9" },
      ],
    };
  },
  components: {
    SingleNote,
  },
};
</script>
<style lang="scss" scoped>
.main-box {
  min-width: 800px;
  min-height: 800px;
  max-width: 900px;
  border: 5px solid rgb(53, 6, 141);
  border-radius: 5px;
  box-shadow: darkgray;
}
.node {
  list-style-type: none;
  // .note-item {
  // min-width: 266px;
  // min-height: 266px;
  // }
}
</style>
