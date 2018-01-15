<template>
<div>
  <el-table
    :data="tableData"
    style=margin-top:2%;width:90%>
    <el-table-column
      prop="stu"
      label="账号">
    </el-table-column>
    <el-table-column
      prop="date"
      label="预约日期">
    </el-table-column>
    <el-table-column
      prop="time"
      label="预约时间">
    </el-table-column>
    <el-table-column
      prop="place"
      label="阅览室">
    </el-table-column>
    <el-table-column
      prop="num"
      label="座位">
    </el-table-column>
  </el-table><br>
  <el-button type="danger" @click="dialogVisible = false" style=margin-left:35% >取 消</el-button>
  <el-button type="primary" @click="dialogVisible = false">提交</el-button>
</div>
</template>

<script>
  export default {
    name: "confirm",
    data() {
      return {
        dialogVisible: false,
        tableData: [{
          stu:'3140602035',
          date: '2018-01-17',
          time: '早上',
          place: '1楼C区',
          num:'23'
        }]

      };
    },

  };
</script>

<style scoped>

</style>
