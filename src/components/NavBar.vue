<script setup>
import NavBarItem from './NavBarItem.vue'
import DocumentationIcon from './icons/IconDocumentation.vue'
import ToolingIcon from './icons/IconTooling.vue'
import EcosystemIcon from './icons/IconEcosystem.vue'
import CommunityIcon from './icons/IconCommunity.vue'
import SupportIcon from './icons/IconSupport.vue'
</script>

<template>
  <NavBarItem>
    <template #icon>
      <DocumentationIcon />
    </template>
    <template #heading>Documentation</template>
  </NavBarItem>

  <NavBarItem>
    <template #icon>
      <DocumentationIcon />
    </template>
    <template #heading>Documentation</template>
  </NavBarItem>


</template>
