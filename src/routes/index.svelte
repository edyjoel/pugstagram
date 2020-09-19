<script context="module">
  export async function preload() {
    let data = [];
    const response = await this.fetch('https://us-central1-pugstagram-co.cloudfunctions.net/data');

    data = await response.json();

    return { data }

  }

</script>

<script>

  import { onMount } from 'svelte';
  import Card from '../components/Card.svelte';

  import Header from '../components/Header.svelte';
  import Main from '../components/Main.svelte';
  import Sidebar from '../components/Sidebar.svelte';
  import Timeline from '../components/Timeline.svelte';

  export let data;

  const API = 'https://us-central1-pugstagram-co.cloudfunctions.net/data';

  // onMount( async () => {

  //   const response = await fetch(API);

  //   data = await response.json();

  //   console.log(data);

  // });

</script>

<svelte:head>
  <title>Pugstagram</title>
</svelte:head>

<Main>
  <Timeline posts={data.posts} />
  <Sidebar />
</Main>