<script>
  let models = [
    { name: "Markus", alter: 25, groesse: "1.85m" },
    { name: "Stefanie", alter: 23, groesse: "1.75m" }
  ];
</script>

<h1>Models</h1>

<ul class="list-group">
  {#each models as model}
    <li class="list-group-item">
      <strong>{model.name}</strong><br />
      Alter: {model.alter} Jahre<br />
      Größe: {model.groesse}
    </li>
  {/each}
</ul>