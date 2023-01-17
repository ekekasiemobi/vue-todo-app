<template>
    <div class=" mx-32 h-56 grid grid-cols-2 gap-4 content-start ...">
      
        <div :key="task.id" v-for="task in tasks" class=" mt-12 w-96 h-48 bg-amber-100 mt-0 content-start" >
            <Task  :task="task" />

        </div>
       
    </div>
    
</template>


<script>
    import Task from './Task'

    export default{
        name: 'Tasks',

        props: {
          tasks: Array,
        },

        components :{
            Task,
        }
    }

</script>

<style scooped>


</style>