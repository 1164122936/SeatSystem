<template>
  <div>
    <div class="num">账号：3140602035</div><br>

    <div class="info">恭喜你已成功预约到座位！</div><br>

      <el-button type="primary" @click="dialogVisible = true">点击查看具体信息</el-button>

      <el-dialog
        title="提示"
        :visible.sync="dialogVisible"
        width="30%"
       >
        <span>2018年1月17日--早上--1楼C区23号座位</span>
        <span slot="footer" class="dialog-footer">
    <el-button type="primary" @click="dialogVisible = false">确 定</el-button>
  </span>
      </el-dialog>

    <el-button type="danger" @click="dialogVisible1 = true">取消预约</el-button>
    <el-dialog
      title="提示"
      :visible.sync="dialogVisible1"
      width="30%"
      >
      <span>是否取消预约2018年1月17日--早上--1楼C区23号座位</span>
      <span slot="footer" class="dialog-footer">
        <el-button type="primary" @click="dialogVisible1 = false">取 消</el-button>
  <el-button type="primary" @click="dialogVisible1 = false">确 定</el-button>
        </span>
    </el-dialog>
  </div>



</template>

<script>
    export default {
        name: "page3",
      data() {
        return {
          dialogVisible: false,
          dialogVisible1: false
        };
      },
    };
</script>

<style scoped>
.num{
  font-size: large;
}
  .info{
    font-size:20px;
  }
</style>
