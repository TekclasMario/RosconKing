<template>
  <v-footer dark height="auto">
    <v-card class="flex" flat tile>
      <v-layout class="footer_layout">
        <v-flex>
          <v-card-title class="page_footer">
            <v-spacer></v-spacer>
            <strong class="subheading page_footer_txt"
              >©2019 Roscon King - All Rights Reserved.</strong
            >
            <v-spacer></v-spacer>
            <v-btn
              id="socmedia"
              v-for="link in links"
              :icon="link.icon"
              :href="link.href"
              target="_blank"
              :key="link.icon"
              class="mx-3"
            >
              <v-icon size="24px">{{ link.icon }}</v-icon>
            </v-btn>
          </v-card-title>
        </v-flex>
        <v-flex class="page_footer">
          <v-card-actions class="mt-4 justify-center">
            &copy;2019 —
            <strong>
              Powered By Tekclas Designs -
              <a href="https://tekclas.com" target="_blank">Tekclas.com</a>
              - All Rights Reserved.
            </strong>
          </v-card-actions>
        </v-flex>
      </v-layout>
    </v-card>
  </v-footer>
</template>

<script>
export default {
  data: () => ({
    links: [
      {
        icon: "fab fa-facebook",
        href: "https://www.facebook.com"
      },

      {
        icon: "fab fa-instagram",
        href: "https://www.instagram.com/roscon_king/"
      }
    ]
  })
};
</script>
