<template>
   <el-input
      class="InputSearch"
      placeholder="Recherche" 
      v-model="input" 
      prefix-icon="el-icon-search">
   </el-input> 
</template>

<script>
export default {
  data() {
    return {
      input: ''
    }
  }
}
</script>