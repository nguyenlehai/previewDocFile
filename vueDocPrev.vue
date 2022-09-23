<template>
  <VueDocPreview :value="docValue" :type="docType" />
</template>
 
<script>
import VueDocPreview from "vue-doc-preview";
export default {
  name: "docvue",
  components: {
    VueDocPreview,
  },
  props: {
    docValue: { type: String },
    docType: { type: String },
  },
};
</script>