<template>
  <v-ons-page>
    <v-ons-navigator :page-stack="pageStack" @push-page="pageStack.push($event)">
          
    </v-ons-navigator>
  </v-ons-page>
</template>


<script>
import Page1 from './Page1'

export default {
  data: function () {
    return {     
      pageStack: [Page1],
    }
  }
}
</script>


