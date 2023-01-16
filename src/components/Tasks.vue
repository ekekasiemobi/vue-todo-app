<template>
    <div class=" mx-32 h-56 grid grid-cols-2 gap-4 content-start ...">
      
        <div class=" mt-12 w-96 h-36 bg-amber-100 mt-0 content-start" :key="task.id" v-for="task in tasks"  >
            <h4>{{task.text}}</h4>
        </div>
       
    </div>

   
   
</template>


<script>
    export default{
        name: 'Tasks',

        props: {
          tasks: Array,
        },

        components :{

        }
    }

</script>

<style scooped>


</style>