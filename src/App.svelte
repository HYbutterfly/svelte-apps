<script context="module">
  import { Router, createRouter } from "@roxi/routify";
  import routes from "../.routify/routes.default.js";

  const router = createRouter({ routes });
</script>

<div id="app">
  <Router {router} />
</div>
