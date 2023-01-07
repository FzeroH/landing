<template>
  <div class="information">
    <p>
      Let’s make something new, different and more meaningful or make thing more visual or conceptual? Just say hello!
    </p>
    <div class="contacts">
      <span>+123 569 789</span>
      <span>youremail@gmail.com</span>
      <span>28 Green Tower, Street name, New York City, USA</span>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Information'
}
</script>

<style lang="scss" scoped>
  .information {
    position: relative;
    p {
      font-size: 2.5rem;
      line-height: 3.25rem;
      max-width: 50rem;
    }
  }
  .contacts {
    position: absolute;
    display: flex;
    flex-direction: column;
    bottom: 0;
    left: 0;

    span {
      position: relative;
      padding-left: 3.8rem;
      font-weight: 300;
      font-size: 1.25rem;
      line-height: 1.5rem;

      &:not(:last-child) {
        padding-bottom: 1rem;
      }

      &::before {
        position: absolute;
        top: 50%;
        left: 0;
        content: '';
        width: 1.375rem;
        height: 1px;
        background: #333333;
      }
    }
  }
</style>
