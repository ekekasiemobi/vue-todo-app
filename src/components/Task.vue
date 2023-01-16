<template>
     <h3>{{task.id}}</h3>
            <h3>{{task.text}}</h3>
            <p>{{task.day}}</p>
            <p>{{task.reminder}}</p>
   

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