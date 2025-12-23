<script>
  import {
    Column,
    Content,
    Grid,
    Header,
    HeaderAction,
    HeaderNav,
    HeaderNavItem,
    HeaderPanelDivider,
    HeaderPanelLink,
    HeaderPanelLinks,
    HeaderUtilities,
    RadioTile,
    Row,
    SideNav,
    SideNavItems,
    SideNavLink,
    SideNavMenu,
    SideNavMenuItem,
    SkipToContent,
    TileGroup,
  } from "carbon-components-svelte";
  import { expoIn } from "svelte/easing";
  import favicon from '$lib/assets/favicon.svg';
  import "carbon-components-svelte/css/all.css";

  let isOpen = $state(false);

  let { children } = $props();
</script>

<Header platformName="Tools of Creation">
  <svelte:fragment slot="skip-to-content">
    <SkipToContent />
  </svelte:fragment>
  <HeaderNav>
    <HeaderNavItem href="/biology" text="Biology" />
    <HeaderNavItem href="/cosmology" text="Cosmology" />
    <HeaderNavItem href="/geography" text="Geography" />
    <HeaderNavItem href="/linguistics" text="Linguistics" />
    <HeaderNavItem href="/planetary" text="Planetary" />
  </HeaderNav>
  <HeaderUtilities>
    <HeaderAction bind:isOpen transition={false}>
      <HeaderPanelLinks>
        <HeaderPanelDivider>Projects</HeaderPanelDivider>
        <HeaderPanelLink>New Project</HeaderPanelLink>
        <HeaderPanelDivider>Actions</HeaderPanelDivider>
        <HeaderPanelLink>Manage Projects</HeaderPanelLink>
      </HeaderPanelLinks>
    </HeaderAction>
  </HeaderUtilities>
</Header>

<Content>
  <Grid>
    <Row>
      <Column>
        {@render children()}
      </Column>
    </Row>
  </Grid>
</Content>
