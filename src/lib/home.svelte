<script lang="ts">
  import home from "../assets/home.svg"
  let time = new Date();
  let sun = time.getDate();
  let mon = sun + 1;
  let tue = mon + 1;
  let wed = tue + 1;
  let thu = wed + 1;
  let fri = thu + 1;
  let sat = fri + 1;
  let month = time.getMonth() +1;
</script>

<div class="topfixed">
    <div class="top">
     <img src={home} class="icon" width="70px" height="70px" alt="">
    </div>
     <div class="Date">
     <div class="date sun">Sun<br>{month}/{sun}</div>
     <div class="date mon">Mon<br>{month}/{mon}</div>
     <div class="date tue">Tue<br>{month}/{tue}</div>
     <div class="date wed">Wed<br>{month}/{wed}</div>
     <div class="date thu">Thu<br>{month}/{thu}</div>
     <div class="date fri">Fri<br>{month}/{fri}</div>
     <div class="date sat">Sat<br>{month}/{sat}</div>
    </div>
    </div>
    <div class="mid">
    <div class="Box">
      <div class="time">00:00 am</div>
      <div class="box">????</div>
     </div>
    <div class="Box">
     <div class="time">00:00 am</div>
     <div class="box">????</div>
    </div>
    <div class="Box">
      <div class="time">00:00 am</div>
      <div class="box">????</div>
     </div>
     <div class="Box">
      <div class="time">00:00 am</div>
      <div class="box">????</div>
     </div>
     <div class="Box">
      <div class="time">00:00 am</div>
      <div class="box">????</div>
     </div>
    <div class="Box">
      <div class="time">00:00 am</div>
      <div class="box">????</div>
    </div>
    <div class="Box">
      <div class="time">00:00 am</div>
      <div class="box">????</div>
    </div>
    <div class="Box">
      <div class="time">00:00 am</div>
      <div class="box">????</div>
    </div>
    <div class="Box">
      <div class="time">00:00 am</div>
      <div class="box">????</div>
    </div>
    <div class="Box">
      <div class="time">00:00 am</div>
      <div class="box">????</div>
    </div>
    <div class="Box">
      <div class="time">00:00 am</div>
      <div class="box">????</div>
    </div>
    <div class="Box">
      <div class="time">00:00 am</div>
      <div class="box">????</div>
    </div>
  </div>
<style>
  .mid{
    overflow: scroll;
  }
  .icon{
    text-align: center;
  }
  .Date{
    position: sticky;
    top: 50px;
    display: flex;
  }
  .date{
    flex-grow: 1;
    padding-top: 10px;
    margin: 7px;
    font-size: 14px;
    flex-direction: row;
    border: 1px solid black;
    background-color: black;
    width: 20px;
    height: 55px;
    color: white;
    border-radius: 20px;
    text-align: center;
    margin-top: 10%;
  }
  .time{
    font-size: 14px;
    border: none ;
    width: 50px;
    height: 15px;
    color:white;
    flex-grow: 1;
    flex-shrink: 1;
  }
  .box{
    border: 5px solid black;
    border: none;
    width: 60%;
    height: 60px;
    background-color: rgba(163, 163, 163, 1);
    border-radius: 15px;
    flex-shrink: 1;
    padding: 10px;
    font-size: 20px;

  }
  .Box{
    display: flex;
    align-items: center;
    margin-top: 10%;
    flex-shrink: 1;
    margin-bottom: 50px;
  }
  
  .top{
    display: flex;
    justify-content: center;
    align-items: center;
  }
</style>