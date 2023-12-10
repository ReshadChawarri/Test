<script>
  import { Card } from "flowbite-svelte";

 
    export let message = "Hello World"
    
    function addExclamation(){
        message += "!"
    }
    </script>
    
    <h1 on:click={addExclamation}>  {message}  </h1>
    <Card>  
     <slot>
        test
     </slot>   
    </Card>
