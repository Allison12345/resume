<template lang="pug">
  .cell
    .cell-hd {{label}}
    .cell-bd {{value}}
</template>
<script>
export default {
  name: "cell",
  props: ["label", "value"]
};
</script>
