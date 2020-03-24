<template>
  <div>

  <div class="sidebar card">
    <div class="sidebar-title card">
      <!-- <h1> Cyber Learning Center </h1>
      <h3> Drexel University Department of Computer Science </h3>
      <h5> Market Room 1066 &#8231; Winter 2020 </h5> -->
    </div>
    <div class="classes">
      <!-- <div class="course"> CS 171: Intro to Programming I <span class="arrow"> >> </span> </div>
      <div class="course"> CS 172: Intro to Programming II <span class="arrow"> >> </span>  </div>
      <div class="course"> SE 181: Software Engineering <span class="arrow"> >> </span>  </div>
      <div class="course"> CS 360: Programming Languages <span class="arrow"> >> </span>  </div> -->
    </div>
  </div>

  <div class="mainview">
    <div class="mainview-title card">

    </div> 
     <!-- <h3> Drexel University Department of Computer Science </h3>
      <h5> Market Room 1066 &#8231; Winter 2020 </h5> -->
    <!-- <div class="timetable">
    <table>
      <tr>
        <th>Company</th>
        <th>Contact</th>
        <th>Country</th>
      </tr>
      <tr>
        <td>Alfreds Futterkiste</td>
        <td>Maria Anders</td>
        <td>Germany</td>
      </tr>
      <tr>
        <td>Centro comercial Moctezuma</td>
        <td>Francisco Chang</td>
        <td>Mexico</td>
      </tr>
      <tr>
        <td>Ernst Handel</td>
        <td>Roland Mendel</td>
        <td>Austria</td>
      </tr>
      <tr>
        <td>Island Trading</td>
        <td>Helen Bennett</td>
        <td>UK</td>
      </tr>
      <tr>
        <td>Laughing Bacchus Winecellars</td>
        <td>Yoshi Tannamuri</td>
        <td>Canada</td>
      </tr>
      <tr>
        <td>Magazzini Alimentari Riuniti</td>
        <td>Giovanni Rovelli</td>
        <td>Italy</td>
      </tr>
    </table> </div> -->
  </div>
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

hr {
  border:none;
  border-top:1px dotted #D0D3D4;
  height:1px;
}
.arrow{
  float: right; 
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

.course{
  margin-top: 1vh; 
  padding: 1vh; 
}

.sidebar{
  position: absolute;
  height: 100%; 
  width: 40vh; 
  background: #34495E; 
  color: white; 
}

.sidebar h3, h5{
  margin-top: -10px;  
}

.sidebar hr{
  color: #F4F6F7; 
}

.sidebar-title{
  height: 10vh; 
  background: #2E4053; 
}

.mainview{
  position: fixed; 
  top: 0px; 
  left: 40vh; 
  right: 0px; 
  bottom: 0px; 
  background: #F8F9F9; 
}

.mainview-title{
  position: fixed; 
  background: white; 
  top: 0px; 
  right: 0px; 
  height: 10vh; 
  left: 40vh; 
 
}



.timetable{
  margin-left: 5vh; 
  margin-top: 5vh; 
  width: 100vh; 
  height: 80vh; 
}




</style>
