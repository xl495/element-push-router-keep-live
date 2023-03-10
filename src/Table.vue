<template>
    <el-table :data="tableData" style="width: 100%" height="300" >
        <el-table-column prop="date" label="Date" width="180" />
        <el-table-column prop="name" label="Name" width="180" />
        <el-table-column prop="address" label="Address" />
    </el-table>
    {{ list }}
    <el-button @click="add" >添加数据</el-button>
</template>


<script lang="ts" setup>
import { ref } from 'vue';

const list = ref<number []>([])

const add = () =>{
    list.value.push(1)
}

    const tableData = [
    {
        date: '1',
        name: 'Tom',
        address: 'No. 189, Grove St, Los Angeles',
    },
    {
        date: '2',
        name: 'Tom',
        address: 'No. 189, Grove St, Los Angeles',
    },
    {
        date: '3',
        name: 'Tom',
        address: 'No. 189, Grove St, Los Angeles',
    },
    {
        date: '4',
        name: 'Tom',
        address: 'No. 189, Grove St, Los Angeles',
    },
    {
        date: '5',
        name: 'Tom',
        address: 'No. 189, Grove St, Los Angeles',
    },
    {
        date: '6',
        name: 'Tom',
        address: 'No. 189, Grove St, Los Angeles',
    },
    {
        date: '7',
        name: 'Tom',
        address: 'No. 189, Grove St, Los Angeles',
    },
    {
        date: '8',
        name: 'Tom',
        address: 'No. 189, Grove St, Los Angeles',
    },
    {
        date: '9',
        name: 'Tom',
        address: 'No. 189, Grove St, Los Angeles',
    },
    {
        date: '10',
        name: 'Tom',
        address: 'No. 189, Grove St, Los Angeles',
    }
]
</script>

<script lang="ts"> 

export default {
    name: 'Table',
}

</script>