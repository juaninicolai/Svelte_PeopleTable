<script>
  import PeopleTable from "./Components/PeopleTable.svelte";
</script>

<main>
  <h1>People Table</h1>
  <h2>Click the 'Generate' button to get random data</h2>
  <h3>If you don't like what you see, just click again!</h3>
  <PeopleTable />
</main>

<style>
  main {
    text-align: center;
    padding: 1em;
    max-width: 240px;
    margin: 0 auto;
  }

  h1 {
    color: #ff3e00;
    text-transform: uppercase;
    font-size: 4em;
    font-weight: 100;
  }

  h2 {
    text-transform: uppercase;
    font-weight: 150;
  }

  h3 {
    text-transform: uppercase;
    font-weight: 150;
  }

  @media (min-width: 640px) {
    main {
      max-width: none;
    }
  }
</style>
