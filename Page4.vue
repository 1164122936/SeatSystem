<template>
  <div>
    <el-table
      :data="tableRecord1"
      style=margin-top:2%;width:90%>
      <el-table-column
        prop="record1"
        label="预约记录">
      </el-table-column>
    </el-table>
      <el-table
        :data="tableRecord2"
        style=margin-top:2%;width:90%>
      <el-table-column
        prop="record2"
        label="黑名单">
      </el-table-column>
    </el-table>
  </div>
</template>

<script>
    export default {
        name: "page4",
      data() {
        return {
          dialogVisible: false,
          tableRecord1: [{
            record1:'预约成功',},
            {
            record1:'预约成功',
          }],
          tableRecord2: [{
            record2:'进入黑名单',},
            {
              record2:'进入黑名单',

          }]
        };
      },
    };
</script>
<style scoped>

</style>


