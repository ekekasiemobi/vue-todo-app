<template>
    
    <h3 class=" pl-6 font-bold pt-6 pr-2">{{task.text}}</h3>
    <p class="text-xs pl-6 pr-2">{{task.day}}</p>
    <h3 class="text-xs pl-6 pr-2">{{task.time}}</h3>
    <p class="text-sm pl-6 font-normal pt-4 pr-2">{{task.reminder}}</p>
   

</template>


<script>
    export default {
        name: 'Task',
        props:{
            task: Object
        }

    }
</script>


<style scoped>

</style>