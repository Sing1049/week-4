<template>
  <div>
    <h2>Hello {{name}}</h2>
    <h3>{{motto}}</h3>
    <h3>{{getMotto}}</h3>
    <p><span>Age:</span>{{ age }}</p>
    <p><span>Color:</span>{{ color }}</p>
  </div>
</template>
<script>
export default {
  props : ["motto"],
  data : function(){
    return{
      name: "Gurjeet",
      age: 21,
      color: "Brown"
    }
  }
}
</script>

<style>
span {
  text-decoration: underline;
  color: sandybrown;
  font-weight: bold;
  transform: uppercase;
  padding-right: 5px;
}
</style>
