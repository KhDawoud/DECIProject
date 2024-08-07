<script lang="ts">
  import {Router, Route} from "svelte-routing";
  import Home from "./lib/pages/Home.svelte";
  import Search from "./lib/pages/Search.svelte";
  import Upload from "./lib/pages/Upload.svelte";
  import AboutUs from "./lib/pages/AboutUs.svelte";
</script>


<Router>
  <Route path="/" component={Home} />
  <Route path="/search" component={Search} />
  <Route path="/upload" component={Upload} />
  <Route path="/about" component={AboutUs} />
</Router>