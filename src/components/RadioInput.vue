<template>

<p>{{ msg }}</p><br/>
<!-- input type free -->
<input type="radio" name="times" class="free" id="times-a" checked>
<label for="times-a">12:00</label>
<input type="radio" name="times" class="free" id="times-b" >
<label for="times-b">12:30</label>
<input type="radio" name="times" class="free" id="times-c" >
<label for="times-c">13:00</label>
<input type="radio" name="times" class="free" id="times-d" >
<label for="times-d">13:30</label>
<!-- input type prime -->
<input type="radio" name="times" class="prime" id="times-e" checked>
<label for="times-e">14:00</label>
<input type="radio" name="times" class="prime" id="times-f" >
<label for="times-f">14:30</label>
<input type="radio" name="times" class="prime" id="times-g" >
<label for="times-g">15:00</label>
<!-- input type free -->
<input type="radio" name="times" class="free" id="times-h" >
<label for="times-h">15:30</label><br/>
<input type="radio" name="times" class="free" id="times-i" >
<label for="times-i">16:00</label>
<!-- input type prenium -->
<input type="radio" name="times" class="prenium" id="times-j" >
<label for="times-j">18:00</label>
<input type="radio" name="times" class="prenium" id="times-k" >
<label for="times-k">18:30</label>
<input type="radio" name="times" class="prenium" id="times-l" >
<label for="times-l">19:00</label>
<input type="radio" name="times" class="prenium" id="times-m" >
<label for="times-m">19:30</label>

</template>

<script>
export default {
  name: 'RadioInput',
  props: {
    msg: String
  }
}
</script>

<style scoped>
label{
    margin-right: 10px;
    margin-top: 2%;
    display: inline-block;

/*CSS pour les input type free*/
}
input[type="radio"].free {
  display: none;
  margin-top: 5%;
  flex-wrap: wrap;
}
input[type="radio"].free + label {
  padding: 2%;
  border: 1px solid #000;
  border-radius: 10px;
}
input[type="radio"].free:checked + label {
  border: 1px solid #000;
  background: black;
  color: white;
}
input[type="radio"].free:hover + label {
  cursor: pointer;
}

/*CSS pour les input type prime*/
input[type="radio"].prime {
  display: none;
  margin-top: 10%
}
input[type="radio"].prime + label {
  padding: 2%;
  border: 1px solid #C12AF9 ;
  border-radius: 10px;
}
input[type="radio"].prime:checked + label {
  border: 1px solid #000;
  background-color: #C12AF9;
  border: 1px solid #fff;
  color: white;
}
input[type="radio"].prime:hover + label {
  cursor: pointer;
}

/*CSS pour les input type prenium*/
input[type="radio"].prenium {
  display: none;
  margin-top: 10%
}
input[type="radio"].prenium + label {
  padding: 2%;
  border: 1px solid #27FC00 ;
  border-radius: 10px;
}
input[type="radio"].prenium:checked + label {
  border: 1px solid #000;
  background-color: #27FC00;
  border: 1px solid #fff;
  color: white;
}
input[type="radio"].prenium:hover + label {
  cursor: pointer;
}


.hello{
  width: 100px;
  height: 100px;
  background-color: blue;
}
#radio{
    width: 50px;
    height: 50px;
    border: 2px;

}
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
