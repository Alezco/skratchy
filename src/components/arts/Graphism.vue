<template>
  <art :art-name="artName"
      :art-categories='graphismCategories'
      :main-title="mainTitle"></art>
</template>

<script>
import Art from '../Art.vue';

export default {
  data() {
    return {
      artName: "graphism",
      mainTitle: "Arts_ Graphiques",
      graphismCategories: [{
          name: "cinquante degrés à l'ombre",
          type: "WAD Magazine",
          class: "wad-mag",
          image: require("../../assets/graphism/wad.jpg"),
          url: "/illustration/electric-animals",
          componentName: "wadContent"
        },
        {
          name: "identité visuelle",
          type: "Restaurant",
          class: "restaurant",
          image: require("../../assets/graphism/restaurant.jpg"),
          componentName: "restaurantContent"
        },
        {
          name: "united movement of benetton",
          type: "benetton",
          class: "benetton",
          image: require("../../assets/graphism/benetton.png"),
          componentName: "benettonContent"
        },
        {
          name: "moma",
          type: "typography",
          class: "moma",
          image: require("../../assets/graphism/moma.png"),
          componentName: "momaContent"
        },
        {
          name: "liberty bell",
          type: "packaging",
          class: "liberty-bell",
          image: require("../../assets/graphism/beer/liberty-thumbnail.jpg"),
          componentName: "beerContent"
        },
        {
          name: "agence de voyage",
          type: "création d'un logo",
          class: "logo-creation",
          image: require("../../assets/graphism/liberty-bell.png"),
          url: "/illustration/electric-animals"
        },
        {
          name: "que sais-je ?",
          type: "livre",
          class: "knowledge",
          image: require("../../assets/graphism/book/know-thumbnail.jpg"),
          componentName: "knowledgeContent"
        },
        {
          name: "basalte",
          type: "persistance rétinienne",
          class: "book-cover",
          image: require("../../assets/graphism/liberty-bell.png"),
          url: "/illustration/electric-animals"
        }
      ]
    };
  },
  components: {
    Art
  }
}
</script>

<style scoped>

</style>
