<script>
  import faker from "@faker-js/faker";
  import TableHead from "./TableHead.svelte";
  import TableRow from "./TableRow.svelte";

  $: rows = [];

  const generateData = () => {
    if (rows.length > 0) {
      rows = [];
    }
    for (let i = 0; i <= 10; i++) {
      rows.push({
        name: faker.name.firstName(),
        email: faker.internet.email(),
        city: faker.address.cityName(),
        zipcode: faker.address.zipCode(),
        country: faker.address.country(),
      });
      rows = rows;
    }
  };
</script>

<table>
  <TableHead />
  <TableRow {rows} />
</table>
<br />
<button on:click={generateData}>Generate</button>

<style>
  table {
    border: 1px solid black;
    margin-left: auto;
    margin-right: auto;
  }
</style>
