<script>
import AppHeader from './components/AppHeader.vue'
import AppContent from './components/AppContent.vue'
import AppFooter from './components/AppFooter.vue'

export default {
  components: {
    AppHeader,
    AppContent,
    AppFooter
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
    <footer>
      <AppFooter />
    </footer>
  </div>

</template>

<style lang="scss">
@use './styles/generals.scss';

</style>
