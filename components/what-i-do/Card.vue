<template>
  <div class="card__container">
    <h1>{{card.title}}</h1>
    <p>{{card.text}}</p>
    <span>
      Read more
      <img src="" alt="">
    </span>
  </div>
</template>

<script>
export default {
  name: 'Card',
  props: {
    card: {
      type: Object,
      default: () => {},
    }
  },
}
</script>

<style lang="scss" scoped>
  .card__container {
    display: flex;
    flex-direction: column;
    background: #333333;
    padding: 4.875rem 2.5rem 0 2.5rem;
    max-width: 23.75rem;

    h1 {
      font-size: 2.875rem;
      line-height: 3.4rem;
      font-weight: 400;
      color: #ffffff;
      margin-bottom: 20px;
      max-width: 300px;
    }

    p {
      font-size: 1.125rem;
      line-height: 1.31rem;
      color: #ffffff;
      max-width: 18.75rem;
    }

    span {
      font-weight: 600;
      font-size: 1.125rem;
      line-height: 1.31rem;
      color: #ffffff;
      padding: 3.75rem 0 2.5rem 0;
      
    }

  }
</style>
