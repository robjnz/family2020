<template>
  <Layout>
    <div id="background" class="container m-auto">
        
        
        <span class="flex content-start">
       
      
      <h1 class="mt-3 text-4xl text-teal-900">
         Shoah Resourses
      
</h1>
 <embed 
          class = "h-12"
          src   = "https://giphy.com/embed/j7N0GKEWqZxNC"  
          alt   = "memorial candle"
         
      />
      </span>
       
       

      <div class="grid sm:flex">
          <auschwitz />
          <austrian />
          <camps />
        
      </div>


      <br />
      <p>
        
        <dropdown />
        
      </p>
      <br />
      <p>
        Add
        <g-link
          class="text-red-600 hover:text-yellow-600"
          to="http://bit.ly/2SxWdgt"
          target="_blank"
        >
          google translate
        </g-link>
        to your browser extensions, to view foreign language web sites.
      </p>

      <br />
    </div>
  </Layout>
</template>

<script>
import auschwitz from "@/components/Shoah/auschwitz";
import austrian from "@/components/Shoah/austrian";
import camps from "@/components/Shoah/camps";

import dropdown from "@/components/Dropdown/dropdown";



export default {
  metaInfo: {
    title: "Shoah",
    meta: [
      {
        name: "description",
        content:
          "Shoah Holocaust Resources",
      },
    ],
  },
  components: {
    auschwitz,
    austrian,
    camps,
    dropdown,
   
  },
};
</script>
