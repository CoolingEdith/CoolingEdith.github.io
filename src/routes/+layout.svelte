<script lang="ts">
  import "../app.postcss";

  // Floating UI for Popups
  import {
    computePosition,
    autoUpdate,
    flip,
    shift,
    offset,
    arrow,
  } from "@floating-ui/dom";
  import {
    storePopup,
    AppShell,
    AppBar,
    LightSwitch,
    modeUserPrefers,
    modeCurrent,
    modeOsPrefers,
  } from "@skeletonlabs/skeleton";
  storePopup.set({ computePosition, autoUpdate, flip, shift, offset, arrow });
</script>

<!-- App Shell -->
<AppShell>
  <svelte:fragment slot="header">
    <!-- App Bar -->
    <AppBar>
      <svelte:fragment slot="lead">
        <strong class="text-xl uppercase">My mix UF</strong>
      </svelte:fragment>
      <svelte:fragment slot="trail">
        <a class="btn btn-sm variant-ghost-surface" href="/recept"> Instruktioner </a>
        <a class="btn btn-sm variant-ghost-surface" href="/order"> Beställ </a>
        <a class="btn btn-sm variant-ghost-surface" href="/info"> Om oss </a>
        <LightSwitch />
      </svelte:fragment>
    </AppBar>
  </svelte:fragment>
  <!-- Page Route Content -->
  <slot />
</AppShell>
