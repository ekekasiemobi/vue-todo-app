<template>
  
  <div style="margin-left:5%; margin-right: 5%;width:90%; height:570px;background-color:white;margin-top:3%" class="drop-shadow-lg">
    <div class="md:grid grid-cols-6">
      <div class="md:col-span-1">
        <Header title="todo-app" />
       
        <Side />
      </div>
      <div class="md:col-span-5">
         <Button />
        <Tasks :tasks="tasks"/>
      </div>
      

    </div> 
    
  </div>
</template>

<script>
import Header from './components/Header'
import Side from './components/Side'
import Tasks from './components/Tasks'
import Button from './components/Button'

export default {
  name: 'App',
  components: {
    Header,
    Side,
    Tasks,
    Button,
  },
  data (){
    return{
      tasks:[

      ]
    }
  },

  created() {
    this.tasks= [
      {
        id: 1,
        text:'Doctors appointment',
        day: 'Monday, January 17, 2023',
        time: '10:00am',
        reminder: 'Work on presentation for client meeting on Wednesday and Prepare dinner',
      },
      {
        id: 2,
        text:'The second task tittle',
        day: 'Tuesday, January 18, 2023',
        time: '4:00pm',
        reminder:' Review and make notes on new industry developments and Yoga class at local studio',
      },
      {
        id: 3,
        text:'The third task tittle',
        day: 'Wednesday, January 19, 2023',
        time:'12:30am',
        reminder:  'Phone call with client to discuss project details and Prepare for upcoming training session',
      }
    ]
  }
 
}
</script>

<style>
body{
  background-color:antiquewhite;
}
/* .container{
  margin-top: 3%;
  margin-left:10%;
  background: red;
} */
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  /* text-align: center; */
  /* background-color: #2c3e50; */
  /* margin-top: 60px; */
}
</style>
