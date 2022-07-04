<script>
  import { Router, Route } from 'svelte-navigator';
  import Index from './pages/Index.svelte';
  import ProjectProtofolio from './pages/projects/Protofolio.svelte'
</script>

<Router primary={false}>
  <Route path="/" component={Index} />
  <Route path="/projects/protofolio" component={ProjectProtofolio} />
</Router>
