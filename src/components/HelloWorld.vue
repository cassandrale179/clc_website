<template>
  <div>

  <div class="sidebar card">
    <div class="sidebar-title card">  
       <h1> Cyber Learning Center </h1> 
    </div>
    <div class="courses">
       <div class="course" v-for="course in courses" :key="course">  
          {{course}}
       </div>
    </div>
  </div>

  <div class="mainview">
    <div class="mainview-title card">
       
    </div> 
    
     <div> 
       <h4> Choose a class on the sidebar to see TA availables and their schedules </h4>
     </div>

    <div class="timetable">
    <table>
      <tr>
        <th v-for="item in headers" :key="item">
          {{ item }}
        </th>
      </tr>
     
      <tr>
        <td>10:00 AM</td>
        <td>
          <ul> 
            <li> Giang Doan </li>
            <li> John Greaves </li>
            <li> Kevin Young </li>
           </ul> 
        </td> 
      
      </tr>
      <tr>
         <td>11:00 AM</td>
        <td>Francisco Chang</td>
        <td>Mexico</td>
      </tr>
      <tr>
        <td>12:00 PM</td>
        <td>Roland Mendel</td>
        <td>Austria</td>
      </tr>
      <tr>
         <td>1:00 PM</td>
        <td>Helen Bennett</td>
        <td>UK</td>
      </tr>
      <tr>
         <td>2:00 PM</td>
        <td>Yoshi Tannamuri</td>
        <td>Canada</td>
      </tr>
      <tr>
        <td>3:00 PM</td>
        <td>Giovanni Rovelli</td>
        <td>Italy</td>
      </tr>
    </table> 
    
    </div>
  </div>
</div>



</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String, 
  }, 
  data(){
    return { 
      courses: [ 'CI 102: Computing and Info II', 'CI 103: Computing and Info III', 
      'CI 492: Senior Design II', 'CS 164: Intro to Computer Science', 
      'CS 171: Programming I', 'CS 172: Programming II', 'CS 260: Data Structure', 
      'CS 265: Advanced Programming Tools & Techniques', 'CS 270: Mathematic Concept for CS', 
      'CS 283: Systems Programming', 
      'CS 303: Cryptography', ],  
      /* 'CS 338', 'CS 342', 'CS 345', 'CS 360', 'CS 370', 
      'CS 375', 'CS 383', 'CS 387', 'CS 432', 'CS 435', 'CS 522', 'CS 525', 
      'CS 530', 'CS 544', 'CS 571', 'CS 613', 'CS 645', 'CS 676', 
      'CS T680', 'SE 181',' SE 211', 'SE 310', 'SE 311', 'SE 410', 'SE 576', 'SE 577'*/ 
      headers: [ 'Time', 'Monday', 'Tuesday', 'Wednesday', 'Thursday', 'Friday'], 
    }
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
.courses{
  padding: 2vh;  
}

.course{
  padding: 1vh; 

}

.sidebar{
  position: absolute;
  height: 100%; 
  width: 40vh; 
  background: #5D6D7E; 
  color: white; 
  z-index: 1000;
}

.sidebar h1{
  margin-top: 13px;  
  font-size: 20px; 
  text-align: center;
}

.sidebar hr{
  color: #F4F6F7; 
}

.sidebar-title{
  height: 6vh; 
  background: #34495E; 
  padding: 2vh; 
}

.mainview{
  position: fixed; 
  top: 0px; 
  left: 40vh; 
  right: 0px; 
  bottom: 0px; 
  background: #F8F9F9; 
  padding-left: 10vh; 
  padding-top: 10vh; 
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
  width: 100vh; 
  height: 80vh; 
}

th{
  background: #808B96; 
  color: white; 
  width: 25vh; 
  height: 5vh; 
}
td{
  width: 25vh; 
  height: 5vh; 
  background: white;
  padding: 1vh;  
}


</style>
