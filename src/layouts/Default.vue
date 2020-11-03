<template>
  <div>
    <a class="visually-hidden" href="#main">Skip to content</a>

    <div id="wrapper" class="wrapper pb-16 md:pb-0 flex flex-col relative min-h-screen bg-teal-200">

      <HeaderPartial/>


      <main id="main" class="main inner flex flex-1 flex-col py-10 lg:py-20">
        <slot/>
      </main>

      <FooterPartial/>
        
    </div>

    <ClientOnly>
    <ResponsiveNav/>
    </ClientOnly>
    
  </div>
</template>

<static-query>
query {
  metadata {
    siteName
  }
}
</static-query>

<script>
import HeaderPartial from '~/layouts/partials/Header.vue'
import FooterPartial from '~/layouts/partials/Footer.vue'
import ResponsiveNav from '~/layouts/partials/ResponsiveNav.vue'

export default {
  script: [

        {src: 'https://kit.fontawesome.com/e3c70d4fc5.js'}
      ],
  components: {
    HeaderPartial,
    FooterPartial,
    ResponsiveNav
  }
}
</script>


<style>

.layout {
  max-width    : auto;
  margin       : 0 auto;
  padding-left : 2px;
  padding-right: 2px;
  background   : #242943;
  color        : #ebf8ff;
  font-size    : 15;

}

.work-card {
            box-shadow   : 0px 0px 20px rgba(0, 0, 0.1);
            padding      : 1rem;
            border-radius: 0.2rem;
            color        : #44337a;
            font-size    : medium;
            font-family: Roberto;
}
#work-card {
  box-shadow: 0px 0px 20px rgba(0, 0, 0.1);
  background: #38b2ac;
  font-family: roberto;
  color: #1a202c;
  font-size: 1.25rem;
}
#background{
    background: #b2f5ea;
}
.postcode{
color     : #68d391;

}

.event{
color     : #4fd1c5;

}

.one{
    color: #e53e3e;
    
  }


</style>