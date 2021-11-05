<template>
    <el-input
    type="text"
    v-model="value"
    :minlength="minlength"
    :maxlength="maxlength"
    :placeholder="placeholder">
    </el-input>
</template>

<script>
export default {
    name: 'InputPrice',
    props: {
        placeholder: { type: String, default: '' },
        minlength: { type: Number, default: 1 },
        maxlength: { type: Number, default: -1 },
    },
    data() {
        return {
        value: '',
        valid: false
        };
    }
};
</script>