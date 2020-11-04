<template>
  <Layout>
    <div id="background" class="container m-auto">
      <h1 class="ml-8 mt-3 text-4xl text-teal-900">
        <span class="text-teal-900">
          <i class="fas fa-theater-masks"></i>
        </span>
        Family History Resourses For Europe
      </h1>
      
      <br />

      <div class="grid sm:flex">
        <austria /><!--Austria-->
        <belarus /><!--Belarus-->
        <belgium /><!--Belgium-->
      </div>

      <div class="grid sm:flex">
        <netherlands />
        <netherlands />
        <netherlands />
      </div>

     
    </div>
    <br />
  </Layout>
</template>

<script>

import austria from "@/components/Europe/austria";
import belarus from "@/components/Europe/belarus";
import belgium from "@/components/Europe/belgium";
import netherlands from "@/components/Europe/netherlands";






export default {
  metaInfo: {
    title: "Europe",
    meta: [
      {
        name: "description",
        content: "A to Z guide of what plays, that are showing at London theatres. Due to coronavirus London theatres are curently closed, new exciting shows coming soon.",
      },
       [

        {src: 'https://kit.fontawesome.com/e3c70d4fc5.js'}
      ],
    ],
  },
  components: {
    austria,
    belarus,
    belgium,
    netherlands,
    
  },
};
</script>

<style></style>
