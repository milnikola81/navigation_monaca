<template>
  <v-ons-page>
    <v-ons-toolbar>
      <div class="left">
        <v-ons-toolbar-button>
          <v-ons-icon icon="ion-more, material:md-more-vert"></v-ons-icon>
        </v-ons-toolbar-button>
      </div>
      <div class="center">My Mobile App</div>
    </v-ons-toolbar>

    <v-ons-tabbar :tabs="tabs">  <!-- can be moved to top with position='top' -->
    </v-ons-tabbar>

  </v-ons-page>
</template>

<script>
import Tab1 from './Tab1'
import Tab2 from './Tab2'

export default {
  data: function () {
      return {
          tabs: [
              {label: 'Tab1', page: Tab1},
              {label: 'Tab2', page: Tab2}
          ]
      }
  }
  
}
</script>


