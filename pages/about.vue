<template>
  <div id="about-page" class="page-wrapper about-page content-page">
    <site-hero
      title="À propos - Become."
      subtitle="`\"Sic itur ad astra\""
      image="/uploads/about-hero.jpg"
    ></site-hero>
    <main-section theme="sidebar-right">
      <template v-slot:default>
        <div class="content">
          <h3>Information</h3>
          <p>
            <strong>
Projet jumelé avec la communauté <a target="_blank" href="https://discord.gg/yWCUap8wej"> Séducquais</a> <br/><br/>

<a target="_blank" href="https://discord.gg/yWCUap8wej"><img src="https://zupimages.net/up/21/04/j7sq.png" alt="" /></a>
          </p>
          <p>
            Site administrer par <a target="_blank" href='Solution#9425' title='Solution'>@Solution</a>
          </p>

        </div>

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
