<script>
  import '../app.css'
</script>

<nav>
  <div>
    <h2>Events App</h2>
    <div>
        <a href="/">Dashboard</a>
        <a href="/todos">Todos</a>
        <a href="/polls">Polls</a>
    </div>
  </div>
</nav>

<main>
    <slot />
</main>
