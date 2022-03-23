<script>
  export let rows;
</script>

{#each rows as row}
  <tr>
    <td><img src={row.pic} alt="avatar" /></td>
    <td>{row.name}</td>
    <td>{row.email}</td>
    <td>{row.city}</td>
    <td>{row.zipcode}</td>
    <td>{row.country}</td>
  </tr>
{/each}

<style>
  td {
    border: 1px solid;
  }
</style>
