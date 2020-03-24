<template>
  <div class="sidebar card">
    <h1> Cyber Learning Center </h1>
    <h3> Drexel University Department of Computer Science </h3>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.sidebar{
  position: absolute;
  height: 100%; 
  width: 40vh; 
  background: #BB8FCE;
  padding-left: 2vh; 
  color: white; 
}

.sidebar h3{
  margin-top: -10px;  
}

.card {
  /* Add shadows to create the "card" effect */
  box-shadow: 0 4px 8px 0 rgba(0,0,0,0.2);
  transition: 0.3s;
}

/* On mouse-over, add a deeper shadow */
.card:hover {
  box-shadow: 0 8px 16px 0 rgba(0,0,0,0.2);
}


</style>
