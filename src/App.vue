<template>
  
  <div style="margin-left:5%; margin-right: 5%;width:90%; height:570px;background-color:white;margin-top:3%" class="drop-shadow-lg">
    <div class="md:grid grid-cols-6">
      <div class="md:col-span-1">
        <Header />
        <Side />
      </div>
      <div class="md:col-span-5">
        <Tasks />
      </div>
    </div> 
    
  </div>
</template>

<script>
import Header from './components/Header'
import Side from './components/Side'
import Tasks from './components/Tasks'

export default {
  name: 'App',
  components: {
    Header,
    Side,
    Tasks,
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
