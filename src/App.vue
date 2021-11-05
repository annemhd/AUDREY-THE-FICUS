<template>
  <div id="app">
    <el-row >
      <el-col :span="18" :offset="4">
        <InputSearch />
        <CheckboxLocation />
        <CheckboxTypes />
        <SelectSize />
        <ButtonPrice />     
        <BaseCard />
      </el-col>
    </el-row>
</div>
</template>

<script>
import InputSearch from './components/filters/InputSearch.vue'
import CheckboxLocation from './components/filters/CheckboxLocation.vue'
import CheckboxTypes from './components/filters/CheckboxTypes.vue'
import SelectSize from './components/filters/SelectSize.vue'
import ButtonPrice from './components/filters/ButtonPrice.vue'
import BaseCard from './components/cards/BaseCard.vue'

export default {
  components: {
    InputSearch,
    CheckboxTypes,
    CheckboxLocation,
    SelectSize,
    ButtonPrice,
    BaseCard
    },
  methods: {
    startHacking () {
      this.$notify({
        title: 'It works!',
        type: 'success',
        message: 'We\'ve laid the ground work for you. It\'s time for you to build something epic!',
        duration: 5000
      })
    }
  }
}
</script>

<style scoped>
#app {
  font-family: Arial, Helvetica, sans-serif;
}
</style>
