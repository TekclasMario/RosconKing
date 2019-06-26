<template>
  <v-carousel vertical hide-delimiters hide-controls>
    <v-carousel-item
      contain
      v-for="(item, i) in items"
      :key="i"
      :src="item.src"
    ></v-carousel-item>
  </v-carousel>
</template>

<script>
export default {
  data() {
    return {
      items: [
        {
          src: "efren.jpg"
        },
        {
          src: "stack.jpg"
        },
        {
          src: "onplate.jpg"
        },
        {
          src: "smallstack.jpg"
        },
        {
          src: "suggar.jpg"
        },
        {
          src: "tableserved.jpg"
        },
        {
          src: "enjoy.jpg"
        },
        {
          src: "coffeenroscon.jpg"
        },
        {
          src: "delish.jpg"
        }
      ]
    };
  }
};
</script>
