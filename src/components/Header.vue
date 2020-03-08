<template>
  <div class="headerStyle">
    <nav>
        <h1>{{ title }}</h1>
        <ul>
          <li><router-link to="/" exact>List</router-link></li>
          <li><router-link to="/add" exact>Add Item</router-link></li>
        </ul>
    </nav>
  </div>
</template>

<script>
export default {
  
  data(){
    return{
        title: 'Grocery List'
        };
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
header {
  background: rgb(122, 63, 100);
  padding: 10px;
  border-style: solid;
  border-color: black;
  border-width: 2px;
}
h1 {
  color: ivory;
}
li {
    list-style-type: none;
    display:inline-block;
    vertical-align: top;
    width: 50%; 
}
.headerStyle{
  background-color: #9d84cb;
  height: 2cm;
}
</style>