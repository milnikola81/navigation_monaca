<template id="Page2">
  <v-ons-page>
    <v-ons-toolbar>
      <div class="left">
        <v-ons-back-button>Page 1</v-ons-back-button>
      </div>
      <div class="center">Page 2</div>
    </v-ons-toolbar>
    <p style="text-align: center">This is the second page</p>

    <br><br>

    <v-ons-button @click="push">Push Page 3</v-ons-button>

  </v-ons-page>
</template>

<script>
import Page3 from './Page3'

export default {
  methods: {
    push() {
      this.$emit('push-page', Page3)
    }
  }
}
</script>


