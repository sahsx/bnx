<template>
  <div class="battle-page">
    <el-table :data="BattleData" style="width: 100%">
      <el-table-column v-for="col in columns" :key="col.prop" v-bind="col">
      </el-table-column>
    </el-table>
  </div>
</template>
<script>
import { ref } from "vue";
import BattleData from "../mock/data.json";

export default {
  setup() {
    const columns = ref([
      {
        prop: "times",
        label: "战斗次数",
        sortable: true,
      },
      {
        prop: "money",
        label: "消耗金币",
      },
      {
        prop: "crystal",
        label: "消耗crystal",
      },
      {
        prop: "attain",
        label: "获得金币",
      },
      {
        prop: "bnx",
        label: "获得bnx",
      },
      {
        prop: "win_times",
        label: "胜利次数",
      },
    ]);
    return {
      columns,
      BattleData,
    };
  },
};
</script>
