<template>
  <div class="hire-me">
    <h1>Hire Me For Your Next Amazing Project</h1>
    <div class="hire-me__content">
      <information />
      <order-form />
    </div>
  </div>
</template>

<script>
import Information from '@/components/hire-me/Information.vue';
import OrderForm from '@/components/hire-me/OrderForm.vue';

export default {
  name: 'HireMe',
  components: { OrderForm, Information }
}
</script>

<style lang="scss" scoped>
  .hire-me {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    width: 100%;

    h1 {
      font-weight: 500;
      font-size: 3.375rem;
      line-height: 4rem;
    }
  }
  .hire-me__content {
    display: flex;
    justify-content: space-around;
    width: 100%;
    margin-top: 80px;
  }
</style>
