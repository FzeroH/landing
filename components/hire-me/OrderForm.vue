<template>
  <form>
    <input type="text" placeholder="Your name">
    <input type="text" placeholder="Your email Address">
    <input type="text" placeholder="Your budget (Optional)">
    <input type="text" placeholder="Your project description">
    <button>Send</button>
  </form>
</template>

<script>
export default {
  name: 'OrderForm'
}
</script>

<style lang="scss" scoped>
  form {
    display: flex;
    flex-direction: column;
    background: #333333;
    padding: 5rem 3.75rem 9.31rem;

    input, input::placeholder {
      font-family: 'Rubik', sans-serif;
      font-style: normal;
      font-weight: 400;
      color: white;
      font-size: 0.875rem;
      line-height: 1.1rem;
    }
    input {
      border: none;
      border-bottom: 1px solid white;
      background: none;
      outline: none;
      padding-bottom: 8px;
      width: 24.1rem;

      &:not(:last-child) {
        margin-bottom: 3.75rem;
      }

    }
    button {
      align-self: end;
      padding: 1rem 2.5rem;
      width: fit-content;
      text-transform: uppercase;
    }
  }
</style>
