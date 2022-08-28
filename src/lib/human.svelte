<script lang="ts">
   import human from "../assets/human.svg"
   import oo from "../assets/oo.svg"
   import xx from "../assets/xx.svg"
</script>
<div class="two">
     <div class="top">
     <img src={human} class="icon" width="60px" height="60px" alt="">
     </div>
     <div class="check notice">
     Notice  <img src={oo} width="44px" height="24px" alt=""> 
     </div>
     <div class = "check vibrate">
     Vibrate <img src={oo} width="44px" height="24px" alt="">
     </div> 
     <div class="check sound">
     Sound <img src={oo} width="44px" height="24px" alt="">
     </div>
</div>
   <style>
    .icon{
      text-align: center;
    }
    .check{
      font-size: x-large;
      color: white;
      margin-top: 50px;
      border: none black;
      background-color: black;
      width: 100%;
      height: 70px;
      text-align: center;
      padding-top: 30px;
    }
    .top{
      display: flex;
      justify-content: center;
      align-items: center;
    }
  </style>