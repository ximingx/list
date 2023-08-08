<script setup>
const tableData = [
  {
    date: '2016-05-03',
    name: 'Tom',
    address: 'No. 189, Grove St, Los Angeles',
  },
  {
    date: '2016-05-02',
    name: 'Tom',
    address: 'No. 189, Grove St, Los Angeles',
  },
  {
    date: '2016-05-04',
    name: 'Tom',
    address: 'No. 189, Grove St, Los Angeles',
  },
  {
    date: '2016-05-01',
    name: 'Tom',
    address: 'No. 189, Grove St, Los Angeles',
  },
]
</script>

<template>
  <div class="container" style="display: flex; flex-direction: column; justify-content: center; align-items: center;">
    <div class="header" style="display: flex; justify-content: center; align-items: center  ;">记事本</div>
    <div class="list">
      <el-table :data="tableData" style="width: 100%">
    <el-table-column prop="date" label="Date" width="180" />
    <el-table-column prop="name" label="Name" width="180" />
    <el-table-column prop="address" label="Address" />
  </el-table>
    </div> 
    <el-pagination background layout="prev, pager, next" :total="12" />
  </div>
</template>

<style scoped>

</style>
