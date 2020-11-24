<template>
  <div >
    <br />
      <div class="border-b-4 border-gray-200"></div>
      <br />

      <br />
      <p>
        <australasia />
        <europe />
        <jewish />
        
      </p>
  </div>
</template>

<script>

import jewish from "@/components/Dropdown/jewish";
import australasia from "@/components/Dropdown/australasia";
import europe from "@/components/Dropdown/europe";

export default {


 components: {
    
    jewish,
    australasia,
    europe,
 }
    
  }
</script>

<style>

</style>