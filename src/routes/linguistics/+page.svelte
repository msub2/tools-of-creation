<script>
  import { SideNav, SideNavItems, SideNavLink } from "carbon-components-svelte";
  let isSideNavOpen = true;
</script>

<SideNav bind:isOpen={isSideNavOpen}>
  <SideNavItems>
    <SideNavLink text="Lexicon" />
    <SideNavLink text="Word Generator" />
    <SideNavLink text="Parts of Speech" />
    <SideNavLink text="Lexical Classes" />
    <SideNavLink text="Grammar" />
    <SideNavLink text="Logographs" />
    <SideNavLink text="Phonology and Text" />
    <SideNavLink text="Phrasebook" />
    <SideNavLink text="Lang Properties" />
    <SideNavLink text="Quiz Generator" />
  </SideNavItems>
</SideNav>