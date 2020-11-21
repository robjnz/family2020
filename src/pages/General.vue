<template>
  <Layout>
    <div id="background" class="container m-auto">
      <h1 class="ml-8 mt-3 text-4xl text-teal-900">
        General Family History Resourses
      </h1>

      <br />

      <div class="grid sm:flex">
        <ancestry />
        <graves />
        <search />
      </div>

      <div class="grid sm:flex">
        <grave />
        <past />
        <geneanet />
      </div>

      <br />
      <div class="border-b-4 border-gray-200"></div>
      <br />

       <h1 class="ml-8 mt-3 text-4xl text-teal-900">
        General Jewish Family History Resourses
      </h1>

       <div class="grid sm:flex">
        <cemeteries />
       </div>
        <br />
      <p>
        <dropdown />
        <jewish />
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
import ancestry from "@/components/General/ancestry";
import graves from "@/components/General/graves";
import search from "@/components/General/search";
import grave from "@/components/General/grave";
import past from "@/components/General/past";
import geneanet from "@/components/General/geneanet";
import cemeteries from "@/components/General/cemeteries";

import dropdown from "@/components/Dropdown/dropdown";
import jewish from "@/components/Dropdown/jewish";

export default {
  metaInfo: {
    title: "General",
    meta: [
      {
        name: "description",
        content:
          "Family history where to find records of birth death and marriages",
      },
    ],
  },
  components: {
    ancestry,
    graves,
    grave,
    search,
    past,
    geneanet,
    cemeteries,

    dropdown,
    jewish,
  },
};
</script>
