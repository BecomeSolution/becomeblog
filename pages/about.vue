<template>
  <div id="about-page" class="page-wrapper about-page content-page">
    <site-hero
      title="À propos - Become."
      subtitle="Sic itur ad astra - Virgile"
      image="/uploads/about-hero.jpg"
    ></site-hero>
    <main-section theme="sidebar-right">
      <template v-slot:default>
        <div class="content">
          <h3>Information</h3>
          <p>
            <strong>
<p> Répertoire utile
Répertoire utile de la communauté Séducquais</a>
Pour plus d'information rejoignez notre discord, <a target="_blank" href="https://discord.gg/yWCUap8wej"> en cliquant ici !s</a>
          </p>
        </div>
</template>
      <template v-slot:sidebar>
        <h3 class="subtitle is-4">
          Latest Posts
        </h3>
        <posts-grid :per-row="1" :number="2" />
      </template>
    </main-section>
  </div>
</template>
<script>
import QuoteCard from '~/components/cards/QuoteCard'
export default {
  head() {
    return {
      title: `À Propos | ${this.$siteConfig.siteName}`
    }
  },
  components: { QuoteCard }
}
</script>
