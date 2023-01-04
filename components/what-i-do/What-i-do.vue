<template>
  <div class="what-i-do">
    <h1>What I Do</h1>
    <div class="test">
      <card :card="card1" class="test__card"/>
      <card :card="card1" class="test__card"/>
      <card :card="card1" class="test__card"/>
    </div>
  </div>
</template>

<script>
import Card from "~/components/what-i-do/Card.vue";

export default {
  name: 'What-i-do',
  components: { Card },
  data() {
    return {
      card1: {
        title: 'UI & UX Design',
        text: 'User interface design, user experience design, user research.',
      },
    }
  },
}
</script>

<style lang="scss" scoped>
  .what-i-do {
    display: flex;
    flex-direction: column;
    align-items: center;
    margin-top: 12.5rem;

    h1 {
      margin-bottom: 3.75rem;
    }
  }
  .test {
    display: flex;
    flex-direction: row;
    margin: 0 2rem;
    .test__card:not(:first-child) {
      margin-left: 7.4rem;
    }

  }

</style>
