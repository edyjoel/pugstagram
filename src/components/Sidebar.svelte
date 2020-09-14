<script>
  import Profile from './Profile.svelte';
  import Stories from './Stories.svelte';
  import Footer from './Footer.svelte';

  export let nickname = "edyjoelx";
  export let name = "Edy Joel"

</script>

<style>
  .Sidebar {
    position: relative;
    padding: 4.5em 0 0 0;
  }
  .Sidebar-container {
    position: fixed;
  }

  @media screen and (max-width: 600px) {
    .Sidebar {
      display: none;
    }
  }
</style>

<div class="Sidebar">
  <div class="Sidebar-container">
    <Profile {nickname} {name} />
    <Stories />
    <Footer />
  </div>
</div>