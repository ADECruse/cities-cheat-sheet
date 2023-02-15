<script lang="ts">
import CardItem from "../CardItem.vue";

export default {
  data(): {} {
    return {};
  },
  components: {
    CardItem,
  },
};
</script>

<template>
  <CardItem>
    <template #title> Links </template>
    <template #contents>
      <p>
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Magni culpa
        eligendi veniam earum autem iste quia ex! Quibusdam dolore dolorum,
        laboriosam culpa nisi consequuntur mollitia, voluptas tempora reiciendis
        ex porro.
      </p>
    </template>
  </CardItem>
</template>
