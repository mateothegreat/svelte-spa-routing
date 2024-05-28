<script lang="ts">
  import { querystring } from "svelte-spa-router";

  // This tells the router to expose the route params to the component
  // as a module-level variable called `params`:
  export let params;

  // This gathers the query string from the router and exposes it to the
  // component as a module-level variable called `queryString`:
  $: queryString = querystring;
</script>

<h1>Foo Component</h1>
<p>Params: {JSON.stringify(params)}</p>
<p>Query string: {$queryString}</p>
