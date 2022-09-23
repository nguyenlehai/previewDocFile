<template>
  <div>
    <p>{{ greeting }} World!</p>

    <VueDocPreview :docValue="text" :docType="type" :height="80" />
  </div>
</template>

<script>
import VueDocPreview from "./vueDocPrev.vue";

export default {
  components: {
    VueDocPreview,
  },
  data: function () {
    return {
      greeting: "BYE..",
      text: "https://static-1252421604.cos.ap-guangzhou.myqcloud.com/vdp.docx",
      type: "office",
    };
  },
};
</script>

<style scoped>
p {
  font-size: 2em;
  text-align: center;
}
</style>