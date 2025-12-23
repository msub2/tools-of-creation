<script>
  import { SideNav, SideNavItems, SideNavLink } from "carbon-components-svelte";
  let isSideNavOpen = true;
</script>

<SideNav bind:isOpen={isSideNavOpen}>
  <SideNavItems>
    <SideNavLink text="Star" />
    <SideNavLink text="Moons" />
    <SideNavLink text="Planet" />
  </SideNavItems>
</SideNav>