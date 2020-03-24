<template>
  <div>

  <div class="sidebar card">
    <div class="sidebar-title card">  
       <h1> Cyber Learning Center </h1> 
    </div>
    <div class="classes">
    
    </div>
  </div>

  <div class="mainview">
    <div class="mainview-title card">
       
    </div> 
    
     <div class="courses"> 
       <h4> Choose a class on the sidebar to see TA availables and their schedules </h4>
     </div>

    <div class="timetable">
    <table>
      <tr>
        <th>Time</th>
        <th>Monday</th>
        <th>Tuesday</th>
        <th>Wednesday</th>
        <th>Thursday</th>
        <th>Friday</th>
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
      items: [ 'CI 102', 'CI 103', 'CI 492', 'CS 164', 
      'CS 171', 'CS 172', 'CS 260', 'CS 265', 'CS 270', 'CS 283', 
      'CS 303', 'CS 338', 'CS 342', 'CS 345', 'CS 360', 'CS 370', 
      'CS 375', 'CS 383', 'CS 387', 'CS 432', 'CS 435', 'CS 522', 'CS 525', 
      'CS 530', 'CS 544', 'CS 571', 'CS 613', 'CS 645', 'CS 676', 
      'CS T680', 'SE 181',' SE 211', 'SE 310', 'SE 311', 'SE 410', 'SE 576', 'SE 577'] 
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
  width: 90%; 
  margin-top: -30px; 
}
.course{
  padding-left: 2vh; 
  padding-right: 2vh; 
  background: #212F3D; 
  display: inline; 
  line-height: 3em; 
  color: white; 
  border-radius: 5px; 
  font-size: 10px; 
  font-family: 'Raleway', sans-serif; 

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
  padding-top: 20vh; 
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
