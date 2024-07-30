<script>
import AppHeader from './components/AppHeader.vue'
import AppContent from './components/AppContent.vue'

export default {
  components: {
    AppHeader,
    AppContent
  }
}
</script>

<template>
  <div>
    <header>
      <AppHeader />
    </header>
    <main>
      <AppContent />
    </main>
  </div>

</template>

<style lang="scss">
@use './styles/generals.scss'

</style>
