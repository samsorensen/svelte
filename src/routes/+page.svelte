<script>
  let events = [
    { id: 1, title: 'Team Meeting', date: '2025-06-02', type: 'meeting' },
    { id: 2, title: 'Project Deadline', date: '2025-06-05', type: 'deadline' },
    { id: 3, title: 'Conference Call', date: '2025-06-08', type: 'call' }
  ];
</script>

<svelte:head>
    <title>Dashboard - Events App</title>
</svelte:head>

<h1>Dashboard</h1>

<div class="dashboard-grid">
  <div class="card">
    <h3>Upcoming Events</h3>
    <div>
      {#each events as event}
        <div class="event-item">
          <span class="event-title">{event.title}</span>
          <span class="event-date">{event.date}</span>
        </div>
      {/each}
    </div>
  </div>
  
  <div class="card stats">
    <h3>Quick Stats</h3>
    <div class="stat-item">
      <p>Total Events: {events.length}</p>
    </div>
    <div class="stat-item">
      <p>This Week: 2</p>
    </div>
  </div>
</div>