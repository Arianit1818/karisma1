<h1>Neues Model erstellen</h1>

{#if success}
  <div class="alert alert-success mt-3">
    Das Model wurde erfolgreich gespeichert!
  </div>
{/if}

<form class="mt-4" method="POST">
  <div class="mb-3">
    <!-- svelte-ignore a11y_label_has_associated_control -->
    <label class="form-label">Name</label>
    <input type="text" class="form-control" name="name" required />
  </div>

  <div class="mb-3">
    <!-- svelte-ignore a11y_label_has_associated_control -->
    <label class="form-label">Alter</label>
    <input type="number" class="form-control" name="alter" required />
  </div>

  <div class="mb-3">
    <!-- svelte-ignore a11y_label_has_associated_control -->
    <label class="form-label">Größe</label>
    <input type="text" class="form-control" name="groesse" required />
  </div>

  <button type="submit" class="btn btn-primary">Speichern</button>
</form>

<script>
  export let form;
  const success = form?.success;
</script>