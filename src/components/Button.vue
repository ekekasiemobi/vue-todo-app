<template>
    <div class=" pt-12 pr-12 flex justify-end ">
        <!-- <button class="justify-end flex">Add task</button> -->
        <a  href="#"><i @click="onClick" class="fa-solid fa-plus"></i></a>
    </div>  
    
</template>


<script>
export default {
    name: 'Button',

    methods:{
        onClick(){
            console.log('click')

        }
    }
}
</script>



<style scoped>

</style>