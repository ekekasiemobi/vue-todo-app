<template>
   <form class=" mx-24 bg-white p-6 rounded-lg">

        <div class="md:grid grid-cols-6">
            <div class="md:col-span-3">
                <label class="block text-gray-700 font-medium mb-2" for="text">Title:</label>
                <input class="w-80 border border-gray-400 p-2 rounded-lg" type="text" id="text" name="text"><br><br>
                <label class="block text-gray-700 font-medium mb-2" for="day">Day:</label>
                <input class="w-80 border border-gray-400 p-2 rounded-lg" type="text" id="day" name="day"><br><br>
            </div>
            <div class="md:col-span-3">
                <label class="block text-gray-700 font-medium mb-2" for="time">Time:</label>
                <input class="w-80 border border-gray-400 p-2 rounded-lg" type="time" id="time" name="time"><br><br>
                <label class="block text-gray-700 font-medium mb-2" for="day">remind:</label>
                <input class="w-80 border border-gray-400 p-2 rounded-lg" type="text" id="day" name="day"><br><br>
            </div>

        </div> 
         <label class="block text-gray-700 font-medium mb-2" for="status">Status:</label>
        <div class="relative rounded-md shadow-sm">
            <select class="form-input py-2 px-3 block w-80 leading-5 rounded-md transition duration-150 ease-in-out bg-white border border-gray-400 focus:border-blue-500 focus:outline-none focus:shadow-outline-blue active:bg-gray-50" id="status" name="status">
            <option value="complete">Complete</option>
            <option value="incomplete">Incomplete</option>
            <option value="on-hold">On-Hold</option>
            <option value="draft">Draft</option>
            </select>
            <div class="pointer-events-none absolute inset-y-0 right-0 flex items-center px-2 text-gray-700">
                <svg class="fill-current h-4 w-4" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 20 20"></svg>
            </div>
        </div><br><br>
        <input class=" w-80 bg-blue-500 text-white p-2 rounded-lg hover:bg-blue-680 text-center mx-56" type="submit" value="Submit">
    </form>

</template>


<script>
export default {
    name: 'Addtask',

    methods:{
        onClick(){
            console.log('click')

        }
    }
}
</script>



<style scoped>

</style>