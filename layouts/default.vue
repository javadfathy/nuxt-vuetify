<script setup>

</script>

<template>
  <VApp>
    <VAppBar scroll-behavior="hide elevate"
          scroll-threshold="89">
      <template v-slot:prepend>
        <VAppBarNavIcon></VAppBarNavIcon>
      </template>

      <VAppBarTitle>Application Bar</VAppBarTitle>

      <template v-slot:append>
        <VBtn icon="mdi-heart"></VBtn>

        <VBtn icon="mdi-magnify"></VBtn>

        <VBtn icon="mdi-dots-vertical"></VBtn>
      </template>
    </VAppBar> 
    <VMain>
      <VContainer>
        <slot />
      </VContainer>
    </VMain>
  </VApp>
</template>