<script>
  import { SideNav, SideNavItems, SideNavLink } from "carbon-components-svelte";
  let isSideNavOpen = true;
</script>

<SideNav bind:isOpen={isSideNavOpen}>
  <SideNavItems>
    <SideNavLink text="Organisms" />
    <SideNavLink text="Tree of Life" />
    <SideNavLink text="Ecosystems" />
  </SideNavItems>
</SideNav>