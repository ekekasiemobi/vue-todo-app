<template>
    <div class=" pt-4 pr-6 flex justify-end ">
        <!-- <button class="justify-end flex">Add task</button> -->
        <a  href="#"><i @click="onClick" class="fa-solid fa-ellipsis-vertical pl-40"></i></a>
    </div>  
    
</template>


<script>
export default {
    name: 'Edit',

    methods:{
        onClick(){
            console.log('click')

        }
    }
}
</script>



<style scoped>

</style>