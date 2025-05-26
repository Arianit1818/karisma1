<script>
  let jobs = [
    {
      titel: "Fotoshooting Sommermode",
      ort: "Zürich",
      datum: "2025-06-15",
      gage: "300 CHF",
      beschreibung: "Shooting für neue Sommerkollektion am Zürichsee."
    },
    {
      titel: "Laufsteg-Event Fashion Week",
      ort: "Mailand",
      datum: "2025-09-02",
      gage: "800 EUR",
      beschreibung: "Laufsteg-Show mit internationalen Designern."
    },
    {
      titel: "Makeup-Werbung",
      ort: "Online",
      datum: "2025-07-01",
      gage: "200 CHF",
      beschreibung: "Kurzvideo für Social Media Kampagne."
    }
  ];
</script>

<h1>Model-Jobs</h1>

<div class="row mt-4">
  {#each jobs as job}
    <div class="col-md-4 mb-3">
      <div class="card h-100">
        <div class="card-body">
          <h5 class="card-title">{job.titel}</h5>
          <h6 class="card-subtitle mb-2 text-muted">{job.ort} – {job.datum}</h6>
          <p class="card-text">{job.beschreibung}</p>
        </div>
        <div class="card-footer">
          <strong>{job.gage}</strong>
        </div>
      </div>
    </div>
  {/each}
</div>