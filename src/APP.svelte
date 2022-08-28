<script lang="ts">
    import home from "./assets/home.svg"
    import human from "./assets/human.svg"
    import HUMAN from "./lib/human.svelte"
    import HOME from "./lib/home.svelte"
  
    let hash: string
    hash = location.hash || '#home'
    $: {
      location.hash = hash
    }
  
  
  </script>
    {#if hash === "#home"}
      <HOME/>
    {:else if hash === "#human"} 
      <HUMAN/>
    {/if}
   <div class="bottom">
     <img  src={home} class="icon" width="50px" height="50px" alt="" on:click={() => {hash = '#home'}}>
     <img src={human} class="icon" width="40px" height="40px" alt="" on:click={() => hash = "#human"}>
   </div>
  <style>
    .icon{
      text-align: center;
    }
    .bottom{
      width:100%;
      height: 50px;
      background-color: black;
      border: 0px solid black;
      border-radius: 10px;
      display: flex;
      justify-content: space-around;
      align-items: center;
      position: fixed;
      bottom: 0px;
      left: 0%;
      right: 0%;
    }
  </style>