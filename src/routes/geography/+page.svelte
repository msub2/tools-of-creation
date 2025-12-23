<script>
  import { SideNav, SideNavItems, SideNavLink } from "carbon-components-svelte";
  let isSideNavOpen = true;
</script>

<SideNav bind:isOpen={isSideNavOpen}>
  <SideNavItems>
    <SideNavLink text="Map Projections" />
    <SideNavLink text="Globe" />
  </SideNavItems>
</SideNav>