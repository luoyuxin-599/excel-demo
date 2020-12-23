<template>
  <div>
    <excel :excelData="excelData" :dataName="dataName"></excel>
  </div>
</template>

<script>
import Excel from "./Excel";
export default {
  data() {
    return {
      excelData: [
        //测试数据
        {
          name: "红烧鱼",
          size: "大",
          taste: "微辣",
          price: "40",
          remain: "100",
        },
        {
          name: "麻辣小龙虾",
          size: "大",
          taste: "麻辣",
          price: "138",
          remain: "200",
        },
        {
          name: "清蒸小龙虾",
          size: "大",
          taste: "清淡",
          price: "138",
          remain: "200",
        }
      ],
      dataName:[{
        name: "名称",
        size: "分量",
        taste: "口味",
        price: "单价",
        remain: "剩余(份)"
      }]
    };
  },
  components: {
    Excel,
  },
};
</script>

<style>

</style>