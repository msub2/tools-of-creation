<script>
  import { SideNav, SideNavItems, SideNavLink } from "carbon-components-svelte";
  let isSideNavOpen = true;
</script>

<SideNav bind:isOpen={isSideNavOpen}>
  <SideNavItems>
    <SideNavLink text="Universe" />
    <SideNavLink text="Galaxy" />
    <SideNavLink text="Magic" />
  </SideNavItems>
</SideNav>