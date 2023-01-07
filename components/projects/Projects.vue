<template>
  <div class="projects">
    <h1>Project</h1>
    <div class="projects__content">
      <p>
        750+
        <span>
          Complited Projects
        </span>
      </p>
      <p>
        15+
        <span>
          On going projects
        </span>
      </p>
      <p>
        250+
        <span>
          Awards
        </span>
      </p>
      <p>
        700+
        <span>
          Happy Clients
        </span>
      </p>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Projects'
}
</script>

<style lang="scss" scoped>
  .projects {
    display: flex;
    position: relative;
    justify-content: center;
    align-items: center;

    h1 {
      position: absolute;
      left: calc(50% - 1093px/2 + 0.5px);
      top: calc(50% - 314px/2 - 21px);
      font-weight: 400;
      font-size: 265px;
      line-height: 314px;
      letter-spacing: 0.13em;
      color: #F1F1F1;
      z-index: -1;

    }
  }
  .projects__content {
    padding: 200px 0;
    display: flex;
    flex-direction: row;
    justify-content: space-evenly;
    width: 100%;

    p {
      display: flex;
      flex-direction: column;
      text-align: center;
      font-size: 4rem;
      line-height: 4.75rem;

      span {
        font-size: 1.5rem;
        line-height: 1.75rem;
      }
    }
  }
</style>
