    <template>
     
     <div class="pa-2 mt-4">
      <v-layout id="mid_section_layout">
        <v-flex xs12 md6>
          <v-img id="mid_section_img_layout"  src="pic_uno.jpg"></v-img>
        </v-flex>

        <v-flex xs12  md6>
          <v-card class="mid_sec_cards"  flat id="card_hover">
            <v-container pa-0>
              <v-layout column>
               
                  <v-card-text class="pa-0">
                    <p  id="body_title" class="text-xs-center">
                      {{ $t("History_Title") }}
                    </p>
                  </v-card-text>

                  <v-card-text >
                    <p id="body_text" class="text-xs-center">{{ $t("History_Content") }}</p>
                  </v-card-text>

              </v-layout>
            </v-container>
          </v-card>
        </v-flex>
      </v-layout>

      <v-layout id="mid_section_layout">
        <v-flex xs12 md6>
          <v-card flat class="mid_sec_cards"  id="card_hover2">
          
              <v-layout column>
               
                  <v-card-text class="black--text">
                    <p id="body_title" class="text-xs-center">
                      {{ $t("Prodcut_Title") }}
                    </p>
                  </v-card-text>

                  <v-card-text >
                    <p id="body_text" class="text-xs-center">{{ $t("Product_Content") }}</p>
                  </v-card-text>
            
              </v-layout>
         
          </v-card>
        </v-flex>
        <v-flex  xs12 md6>
          <v-img id="mid_section_img_layout" src="pic_doz.jpg"></v-img>
        </v-flex>
      </v-layout>

      <v-layout id="mid_section_layout">
        <v-flex xs12 md6>
          <v-img id="mid_section_img_layout"  src="pic_tres.jpg"></v-img>
        </v-flex>

        <v-flex xs12 md6>
          <v-card class="mid_sec_cards"  flat id="card_hover3" >
            <v-container>
              <v-layout column>
              
                  <v-card-text pa-0 class="pa-0 black--text">
                    <p  id="body_title" class="text-xs-center">
                      {{ $t("Vision_Title") }}
                    </p>
                  </v-card-text>

                  <v-card-text class="pa-0 grey--text">
                    <p id="body_text"  class="text-xs-center">{{ $t("Vision_Content") }}</p>
                    <p id="body_text"  class="black--text text-xs-center">
                      <strong>{{ $t("Vision_Footer") }}</strong>
                    </p>
                  </v-card-text>

                  <div class="text-xs-center">
                 <Popup />
                  </div>
            
              </v-layout>
            </v-container>
          </v-card>
        </v-flex>
      </v-layout>
    </div>
    
   </template>
   
 