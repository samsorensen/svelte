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

<div>
  <div>
    <h3>Upcoming Events</h3>
    <div>
      {#each events as event}
        <div>
          <span>{event.title}</span>
          <span>{event.date}</span>
        </div>
      {/each}
    </div>
  </div>
  
  <div>
    <h3>Quick Stats</h3>
    <p>Total Events: {events.length}</p>
    <p>This Week: 2</p>
  </div>
</div>