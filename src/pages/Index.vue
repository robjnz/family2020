<template>
  <Layout>
    <section id="container-centre" class="column centre flex-1">
      <h1 class="page-title">Welcome to Family History</h1>
      <div class="content">
        <p>What records are available, and where to find usefull family history records.</p>
       
        <div class="grid sm:flex">
       
        <g-image
          class="object-fill"
          src="@/images/logotreerobin.svg" width="400"
          alt="logo"
        />
        <br />
        
        <ul class="mb-12 list-disc pl-4">
          <li>
            Births records
          </li>
          <li>School records</li>
          <li>Marriage records</li>
          <li>Death records</li>
          <li>Burial records</li>
          <li>Will and Probate records</li>
          <li>Census records</li>
          <li>Electoral roll</li>
          <li>Military records</li>
          <li>Immigration & Travel records</li>
        </ul>
        </div>
        
        <br /><br />
       
      
      </div>
    </section>
  </Layout>
</template>

<script>
export default {
  metaInfo: {
    title: "Home",
  },
};
</script>
