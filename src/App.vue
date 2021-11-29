<template>
  <form action="" method="get">
<DateInput msg="Select a day"/>

<RadioInput msg="Choose one of the available timeslots"/>

<div id="info">
<b>Info about available timeslots</b>
<ul>
<li>Regular slots</li>
<h5>Free</h5>
<li id="green">Prenium slots</li>
<h5>INR 134</h5>

<li id="purple">Primes slots</li>
<h5>INR 254</h5>
</ul>
</div>

</form>
<HelloWorld msg="hello "/>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import DateInput from './components/DateInput.vue'
import RadioInput from './components/RadioInput.vue'
console.log("Hello world !")

export default {
  name: 'App',
  components: {
    HelloWorld,
    DateInput,
    RadioInput,
  }
}
</script>

<style>
#green{
  color:#27FC00;
}
#purple{
  color: #C12AF9;
}
ul{
  display: flex;
}
#info{
  background-color: #C7F1F7;
  border-radius: 10px;
  padding: 2%;
  margin-top: 5%;
  bottom: 2%;
}

form{
  box-shadow: rgba(0, 0, 0, 0.35) 0px 5px 15px;
  border-radius: 10px;
  height: 500px;
  padding-top: 3%;
  padding-left: 3%;
  padding-right: 3%;
  margin-right: 25%;
  margin-left: 25%;
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
