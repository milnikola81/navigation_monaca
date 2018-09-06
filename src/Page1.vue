<template id="Page1">
  <v-ons-page>
    <v-ons-toolbar>
      <div class="center">Page 1</div>
    </v-ons-toolbar>
    <p style="text-align: center">
      This is the first page
    </p>

    <br><br>

    <v-ons-button @click="push">Push Page 2</v-ons-button>

  </v-ons-page>
</template>

<script>
import Page2 from './Page2'

export default {
  methods: {
    push() {
      this.$emit('push-page', Page2);
    }
  }
}
</script>
