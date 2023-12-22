<script setup>
import { ref } from 'vue';

const props = defineProps({
    employees: Array
}); 

const print = () => {
    console.log(props.employees);
}
</script>

<template>
    <div class="empoloyee-list">
        <div class="empoloyee-item" v-for="(item, index) in props.employees" :key="index">{{ item.name }}</div>
    </div>
</template>

<style scoped>
    .empoloyee-item {
        background-color: #fff;
        padding: 15px;
        margin: 5px;
        border-radius: 3px;
        border: 1px solid #ccc;
    }
</style>