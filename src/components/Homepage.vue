<template>
  <Header style="margin-bottom: 30px;"/>
  <Card />
</template>

<script>
import Header from "./Header.vue";
import Card from "./Card.vue";

export default {
  name: "App",
  components: {
    Header,
    Card
  },
};
</script>
