<template>
  <div class="container bg-black">
    <div class="w-full mx-16">
      <CaseEntry 
      v-for="projectInfo in projectInfo"
      :key="projectInfo.id"
      :projectInfo="projectInfo"
      />
    </div>
  </div>
</template>

<script>
import CaseEntry from '~/components/CaseEntry.vue'
import {projectInfo} from "@/assets/data/projects.js"
export default {
  data() {
    return {
      projectInfo: projectInfo
    }
  }
}
</script>

<style>
/* Sample
CaseEntry `apply` at-rules with Tailwind CSS
.container {
@apply min-h-screen flex justify-center items-center text-center mx-auto;
}
*/
.container {
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}

.title {
  font-family: 'Quicksand', 'Source Sans Pro', -apple-system, BlinkMacSystemFont,
    'Segoe UI', Roboto, 'Helvetica Neue', Arial, sans-serif;
  display: block;
  font-weight: 300;
  font-size: 100px;
  color: #35495e;
  letter-spacing: 1px;
}

.subtitle {
  font-weight: 300;
  font-size: 42px;
  color: #526488;
  word-spacing: 5px;
  padding-bottom: 15px;
}

.links {
  padding-top: 15px;
}
</style>
