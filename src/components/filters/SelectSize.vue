<template>
    <el-popover
      placement="bottom"
      trigger="click"
      >
        <el-select v-model="value" placeholder="Select">
            <el-option
            v-for="item in sizes"
            :key="item"
            :label="item"
            :value="item">
            </el-option>
        </el-select>
        <el-button slot="reference">Taille</el-button>
    </el-popover>
</template>

<script>
  const sizeOptions = ['Petit', 'Moyen', 'Grand'];
  export default {
    data() {
      return {
        sizes: sizeOptions,
        value: ''
      };
    }
  };
</script>