<script lang="ts">
  import Router, { link } from "svelte-spa-router";
  import { routes } from "./routes";
</script>

Click <a use:link={"/rooms/q234f34g?asdf=sadf"}>http://localhost:5173/#/rooms/q234f34g?asdf=sadf</a>

<hr>

<Router {routes} />
