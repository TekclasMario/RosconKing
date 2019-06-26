<template>
  <div >
    <!-- top section  -->

    <!-- Mid_Section -->

    <div id="red-banner">
      <h1 class="text-xs-center pt-2 white--text">{{ $t("About") }}</h1>
    </div>


    <div class="mt-5" id="red-banner">
      <h1 class="text-xs-center pt-2 white--text">{{ $t("Flavors") }}</h1>
    </div>

   
    <div class="mt-1 pa-2" id="red-banner">
      <h1 class="text-xs-center white--text">{{ $t("Info") }}</h1>
    </div>
    
    
    
   
  </div>
</template>

<script>

import Carousel from "@/components/Carousel";

export default {
  components: {
    
    Carousel
  },
  props: {
    msg: String
  }
};

</script>;
