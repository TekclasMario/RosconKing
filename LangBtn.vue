<template>
  <v-layout align-content-center justify-center colum>
    <v-btn
      v-for="entry in languages"
      :key="entry.title"
      @click="changeLocale(entry.language)"
      Medium
      color="#CB4154"
      class="white--text"
      >{{ entry.title }}</v-btn>
  </v-layout>
</template>

<script>
import i18n from "@/plugins/i18n";
export default {
  data() {
    return {
      languages: [
        { flag: "us", language: "en", title: "English" },
        { flag: "es", language: "es", title: "Español" }
      ]
    };
  },
  methods: {
    changeLocale(locale) {
      i18n.locale = locale;
    }
  }
};
</script>
