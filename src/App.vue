<template>
  <div id="app" class="container">  
  <div class="row">
  <project-vuex />
  </div> 
   <br>
      <div class="row py-4">
      <project-cv-2 />
      </div>
    </div>
</template>

<script>

import ProjectVuex from './components/ProjectVuex.vue';
import ProjectCv2 from './components/ProjectCv2.vue';

export default {
  name: "App",
  components: {
    ProjectVuex,
    ProjectCv2,
  },
};

</script>