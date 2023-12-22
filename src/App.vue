<script setup>
import Header from './components/Header.vue'
import EmployeesList from './components/EmployeesList.vue';

const employees = ([
    {name: 'Alex'},
    {name: 'Nikolas'},
    {name: 'Mile'},
    {name: 'Papay'},
    {name: 'Ivan'},
    {name: 'Yuriy'}
]);

</script>


<template>
    <header class="header">
        <Header />
    </header> 

    <main class="main">
        <EmployeesList :employees="employees" />
    </main>
    
</template>

<style scoped>
    .header,
    .main {
        background-color: #a8d8ff;
        padding: 20px;
        border-radius: 5px;
        box-shadow: 0 5px 10px #dedede;
        margin-bottom: 20px;
    }
    .main {
        background-color: #ffd700;
        padding: 20px;
        border-radius: 5px;
        box-shadow: 0 5px 10px #dedede;
        margin-bottom: 20px;
    }
    
</style>