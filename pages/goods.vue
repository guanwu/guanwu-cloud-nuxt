<template>
    <div>
      <h2>商品信息</h2>
      
      <!-- Control Buttons -->
      <el-button-group>
        <el-button type="primary" @click="addRow">新增</el-button>
        <el-button type="primary" @click="copyRow">复制</el-button>
        <el-button type="danger" @click="deleteRow">删除</el-button>
      </el-button-group>
  
      <!-- Table -->
      <el-table :data="items" border style="margin-top: 20px; width: 100%">
        <el-table-column prop="number" label="项号" width="50"></el-table-column>
        <el-table-column prop="code" label="商品编号" width="150">
          <template #default="scope">
            <el-input v-model="scope.row.code"></el-input>
          </template>
        </el-table-column>
        <el-table-column prop="name" label="商品名称及规格型号">
          <template #default="scope">
            <el-input v-model="scope.row.name"></el-input>
          </template>
        </el-table-column>
        <el-table-column prop="quantity" label="数量及单位">
          <template #default="scope">
            <el-input-number v-model="scope.row.quantity" :min="0"></el-input-number>
            <el-select v-model="scope.row.unit" placeholder="单位">
              <el-option label="千克" value="KG"></el-option>
              <el-option label="克" value="G"></el-option>
            </el-select>
          </template>
        </el-table-column>
        <el-table-column prop="price" label="单价/总价/币值">
          <template #default="scope">
            <el-input-number v-model="scope.row.price" :min="0"></el-input-number>
            <el-input v-model="scope.row.currency"></el-input>
          </template>
        </el-table-column>
        <!-- Add more columns as needed based on your design -->
      </el-table>
  
      <!-- Footer Totals -->
      <div style="margin-top: 10px;">
        <span>毛重: {{ totalWeight }} KG</span>
        <span>净重: {{ totalNetWeight }} KG</span>
        <span>总金额: {{ totalAmount }}</span>
      </div>
    </div>
  </template>
  
  <script>
  import { ref, computed } from 'vue';
  import { ElMessage } from 'element-plus';
  
  export default {
    setup() {
      const items = ref([
        { number: 1, code: '', name: '', quantity: 0, unit: 'KG', price: 0, currency: '人民币' }
      ]);
  
      const addRow = () => {
        items.value.push({ number: items.value.length + 1, code: '', name: '', quantity: 0, unit: 'KG', price: 0, currency: '人民币' });
      };
  
      const copyRow = () => {
        if (items.value.length > 0) {
          const lastItem = items.value[items.value.length - 1];
          items.value.push({ ...lastItem, number: items.value.length + 1 });
        }
      };
  
      const deleteRow = () => {
        if (items.value.length > 0) {
          items.value.pop();
        } else {
          ElMessage.warning("没有更多行可删除");
        }
      };
  
      const totalWeight = computed(() => items.value.reduce((acc, item) => acc + item.quantity, 0));
      const totalNetWeight = computed(() => items.value.reduce((acc, item) => acc + item.quantity, 0));
      const totalAmount = computed(() => items.value.reduce((acc, item) => acc + item.price, 0));
  
      return { items, addRow, copyRow, deleteRow, totalWeight, totalNetWeight, totalAmount };
    }
  };
  </script>
  
  <style scoped>
  /* Add any necessary styling here */
  </style>
  