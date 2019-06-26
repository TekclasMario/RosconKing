<template>
  
    <v-layout id="top_section">
 
      <v-flex xs12 md7>
   
        <v-img width="100%" src="OfficialBanner.png"> </v-img>
      
   
    </v-flex>
     
    <v-flex class="banner-text-box" xs12 md5  align-self-center>
                 
                  <v-card-text class="banner_title white--text">
                    <p class="text-xs-center">
                      {{ $t("Banner_Main") }}
                    </p>
                  </v-card-text>
               
                <v-card-text class="banner_text grey--text">
                  <p class="text-xs-center">
                    <strong>{{ $t("Banner_Secndary_Bold") }}</strong>
                    {{ $t("Banner_Secondary") }}
                  </p>
                </v-card-text>
                <LangBtn />
              </v-flex>
   
     </v-layout>
        
   

    </template>
    
   
  <script>
 import LangBtn from "@/components/LangBtn";
      
      export default {
  components: {
    
    LangBtn
  },
  props: {
    msg: String
  }
};
      
      
      </script>




