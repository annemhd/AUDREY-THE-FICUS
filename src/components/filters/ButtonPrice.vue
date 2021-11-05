<template>
    <el-popover
        placement="bottom"
        trigger="click"
        style="width:100px"
    >
        <InputPrice :placeholder="'min'"/>
        <InputPrice :placeholder="'max'" />
        <el-button slot="reference">Prix</el-button>
    </el-popover>
</template>

<script>
import InputPrice from '/Users/amichaud/Documents/GitHub/AUDREY-THE-FICUS/src/components/filters/InputPrice.vue'

export default {
    name: 'ButtonPrice',
   components: {
       InputPrice
   }
};
</script>

<style scoped>
.el-input {
    width: 100px;
}
</style>