<template>

<label>{{ msg }}</label><br />
<input id="date" type="date" value="29/11/2021">


</template>

<script>
export default {
  name: 'DateInput',
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
#date{
    width: 100%;
    margin-top: 2%;
    margin-bottom: 5%;
}
.hello{
  width: 100px;
  height: 100px;
  background-color: blue;
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
