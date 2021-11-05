<template>
    <el-popover
      placement="bottom"
      trigger="click"
      >
      <el-checkbox-group
      class="CheckboxTypes"
        v-model="checkedPlants"
        :max="5"
      >
          <el-checkbox 
            v-for="plant in plants" 
            :label="plant" 
            :key="plant"
            > 
            {{plant}} 
            </el-checkbox>
      </el-checkbox-group>
      
        <el-button slot="reference">Types de plantes</el-button>
    </el-popover>
</template>

<script>
  const plantOptions = ['Ficus', 'Calathea', 'Bambou', 'Aloe Vera'];
  export default {
    data() {
      return {
        checkedPlants: [],
        plants: plantOptions,
        visible: false
      };
    }
  };
</script>
