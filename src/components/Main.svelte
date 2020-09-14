<style>
  .Main {
    display: grid;
    grid-template-columns: minmax(auto, 936px);
    justify-content: center;
    background-color: #fafafa;
  }
  .Main-container {
    display: grid;
    grid-template-columns: 3fr 1fr;
    grid-gap: 2em;
    padding: 2em 0;
  }

  @media screen and (max-width: 600px) {
    .Main-container {
      grid-template-columns: auto;
      padding: 2em 2em;
    }
  }
</style>

<div class="Main">
  <div class="Main-container">
    <slot />
  </div>
</div>