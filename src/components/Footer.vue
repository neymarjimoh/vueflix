<template>
  <v-card height="150">
    <v-footer absolute class="font-weight-normal">
      <v-col class="text-center" cols="12">
        &copy; {{ new Date().getFullYear() }} — Made with
        <v-btn class="ml-1" text icon color="pink">
          <v-icon>mdi-heart</v-icon>
        </v-btn>
        <span class="ml-1 footer__username">by <strong>Jimmy</strong></span>
      </v-col>
    </v-footer>
  </v-card>
</template>

<script>
export default {};
</script>

<style scoped>
a:-webkit-any-link {
  text-decoration: none;
}
.footer__username {
    font-family: gil;
}
</style>
