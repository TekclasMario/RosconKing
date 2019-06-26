<template>
  <div id="app" class="foundation_color">
    <Top_Section/>

    <div id="Divider_Color">
      <p class="text-xs-center white--text">{{ $t("About") }}</p>
    </div>
    <Mid_Section/>
    <div id="Divider_Color">
      <p class="text-xs-center white--text">{{ $t("Flavors") }}</p>
    </div>

    <div class="mt-5 mb-5">
      <v-img width="100%" src="flavors.png"></v-img>
    </div>

    <Carousel class="mb-5"/>
    <div id="Divider_Color">
      <p class="text-xs-center white--text">{{ $t("Info") }}</p>
    </div>

    <Bottom_Section/>

    <Footer/>
  </div>
</template>

<script>
import Top_Section from "./components/Top_Section";
import Mid_Section from "./components/Mid_Section";
import Bottom_Section from "./components/Bottom_Section";
import Carousel from "./components/Carousel";

import Footer from "./components/Footer";
import i18n from "@/plugins/i18n";

export default {
  name: "app",
  components: {
    Top_Section,
    Mid_Section,
    Bottom_Section,
    Carousel,
    Footer
  },
  data() {
    return {
      languages: [
        { language: "en", title: "English" },
        { language: "es", title: "Español" }
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

<style>
/* Foundation section */

.foundation_color {
  background-color: #fffde7;
  transition: 20s linear;
}

.foundation_color:hover {
  background-color: #ef9a9a;
}

a {
  text-decoration: none;
  color: white;
  transition: 0.8s linear;
}

a:hover,
.page_footer_txt:hover {
  color: black;
}

#red-banner {
  background-color: #cb4154;
  height: 57.1px;
}

/* top section */

#top_section {
  flex-direction: row;
  background-color: black;
}

.banner_title {
  font-family: "Vollkorn", Times, serif;
  font-size: 30px;
  font-weight: bold;
}

.banner_text {
  font-family: "Vollkorn", Times, serif;
  font-size: 16.5px;
}

.banner-text-box {
  padding: 2.5rem;
  background-color: black !important;
}

/* mid section */

#Divider_Color {
  background-color: #cb4154;
  height: 88.8px;
  font-size: 2rem;
  padding: 1.9rem;
}

#card_hover,
#card_hover2,
#card_hover3,
.page_footer_txt {
  transition: 0.8s linear;
}

#card_hover {
  background-color: #e8eaf6;
}

#card_hover2 {
  background-color: #fce4ec;
  color: grey;
}

#card_hover:hover {
  background-color: #ef9a9a;
  color: white;
}

#card_hover2:hover {
  background-color: #ffecb3;
}

#card_hover3:hover {
  background-color: #f1f8e9;
}

#mid_section_layout {
  padding-top: 8px;

  margin-top: 8px;
  margin-bottom: 38px;
  display: flex;
  flex-direction: row;
}

.mid_sec_cards {
  padding-top: 3.5rem;
  height: 100%;
}

#mid_section_img_layout {
  height: 100%;
}

#body_title {
  font-family: "Helvetica Neue", Helvetica, Arial, sans-serif;
  font-size: 25px;
  font-weight: bold;
}

#body_text {
  font-family: "Helvetica", Helvetica, Arial, sans-serif;
  font-size: 18.5px;
  padding-left: 2rem;
  padding-right: 2rem;
}

.flavors_section {
  padding: 30px 0 30px 0;
  width: 100%;
}

/* bottom section */

#bottom_text {
  background-color: #fce4ec;
}

#bottom_text .body_text {
  transition: 0.8s linear;
  color: grey;
}

#bottom_text .body_text:hover {
  color: black;
}

/* footer */

.page_footer {
  background-color: #ef9a9a;
}
.footer_layout {
  flex-direction: row;
}

#socmedia:hover {
  color: black;
}

/* Media Queries */

@media screen and (max-width: 1024px) {
  #top_section {
    flex-direction: row;
  }
  #top_section_layout {
    padding: none;
  }

  .banner-text-box {
    padding: 1rem;
  }

  /* mid section */

  .body_text {
    font-family: "Helvetica", Helvetica, Arial, sans-serif;
    font-size: 13.5px;
  }

  #mid_section_layout {
    display: flex;
    flex-direction: row;
    padding-top: 1rem;
    margin-top: 0;
  }

  #mid_section_img_layout {
    padding-top: 0;
  }

  /* flavors section */

  .flavors_section {
    padding: 0 0 0 0;

    max-width: 100%;

    object-fit: contain;
  }

  /* footer section */

  .footer_layout {
    flex-direction: row;
  }

  #socmedia {
    padding-left: 7rem;
  }
}

/* End or this query section */

@media screen and (max-width: 959px) {
  .banner-text-box {
    padding: 0rem;
  }
}

@media screen and (max-width: 888px) {
  /*    Top Section*/

  #top_section {
    flex-direction: column;
  }

  #top_section_layout {
    padding: none;
  }

  .banner-text-box {
    padding: 3rem 0rem 4rem 0rem;
  }

  .banner_title {
    font-size: 25px;
    padding: 0rem;
  }

  .banner_text {
    font-size: 12.5px;
  }

  /* mid section */

  #card_hover3 {
    padding: 0;
  }

  #mid_section_layout {
    display: flex;
    flex-direction: column;
    padding-top: 1rem;
    margin-top: 0;
  }

  #mid_section_img_layout {
    margin-top: 1rem;
    margin-bottom: 1rem;
    padding-top: 1rem;
    height: 30rem;
  }

  .mid_sec_cards {
    padding-top: 1rem;
    height: 15rem;
  }

  #body_title {
    padding-top: 0.3rem;
    padding-bottom: 0.2rem;
    font-size: 25.5px;
  }

  #body_text {
    font-family: "Helvetica", Helvetica, Arial, sans-serif;
    font-size: 12.5px;
    margin: 0.2rem;
  }

  /* flavors section */

  .flavors_section {
    padding: 0 0 0 0;

    max-width: 100%;

    object-fit: contain;
  }

  /* footer section */

  .footer_layout {
    flex-direction: column;
  }

  #socmedia {
    padding-left: 7rem;
  }
}

/* End or this query section */

@media screen and (max-width: 719px) {
  .banner-text-box {
    padding: 2rem 0rem 2rem 0rem;
  }

  .banner_title {
    font-size: 1.3rem;
  }

  .banner_text {
    font-size: 0.8rem;
  }

  /* mid section */

  #mid_section_layout {
    display: flex;
    flex-direction: column;
  }

  #body_title {
    font-size: 1.1rem;
    padding-top: 1.6rem;
    padding-bottom: 0.5rem;
  }

  #body_text {
    font-size: 10.5px;
    padding: 0.5rem 1rem 1rem 1rem;
    margin: 0;
  }

  .mid_sec_cards {
    height: 90%;
    padding-top: 0;
  }

  #mid_section_img_layout {
    height: 90%;
    padding-top: 0;
  }
}

@media screen and (max-width: 600px) {
  /*Top Section    */

  #top_section {
    flex-direction: column;
  }

  #top_section_layout {
    padding: none;
  }

  .banner-text-box {
    padding: 1.7rem 1.7rem 3rem 1.7rem;
  }

  .banner_title {
    font-size: 2rem;
  }

  .banner_text {
    font-size: 1.3rem;
  }

  /* mid section */

  #mid_section_layout {
    display: flex;
    flex-direction: column;
    padding-top: 1rem;
    margin-top: 0;
  }

  .body_text {
    font-family: "Helvetica", Helvetica, Arial, sans-serif;
    font-size: 13.5px;
  }

  #mid_section_img_layout {
    padding-top: 1rem;
  }

  .mid_sec_cards {
    padding-top: 1rem;
  }

  /* flavors section */

  .flavors_section {
    padding: 0 0 0 0;

    max-width: 100%;

    object-fit: contain;
  }

  /* footer section */

  .footer_layout {
    flex-direction: column;
  }

  #socmedia {
    padding-left: 7rem;
  }
}
</style>
