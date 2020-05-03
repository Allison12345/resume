<template lang="pug">
.resume
  .resume-hd
    .resume-hd__left
      Cell(v-for="(item,index) in resumeHdItems" :key='index' :label='item[label]' :value='itme[value]')
    .resume-hd__right
      image(src='')
  .resume-bd
</template>
<script>
import Cell from "@/components/cell/index.vue";
export default {
  name: "resume",
  components: {
    Cell
  },
  data() {
    return {
      resumeHdItems: [
        { label: "姓名", value: "吴川平" },
        { label: "年龄", value: "22" },
        { label: "电话", value: "电话" },
        { label: "地址", value: "贵阳市花溪区" },
        { label: "邮箱", value: "2562392373@qq.com" }
      ]
    };
  }
};
</script>
<style lang="less">
.resume {
  width: 100%;
  height: 100%;
}
</style>
