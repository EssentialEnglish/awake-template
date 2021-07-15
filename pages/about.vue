<template>
  <div id="about-page" class="page-wrapper about-page content-page">
    <site-hero
      title="About"
      subtitle="Essential English"
      image="/uploads/about-hero.jpg"
    ></site-hero>
    <main-section theme="sidebar-right">
      <template v-slot:default>
        <div class="content">
          <h3>Who are we?</h3>
          <p>
          </p>
          <p>
            We are experienced English teachers who want learners to be able to meet other learners from around the world and discuss important and intersting issues.
            We encourage you to use our Slack room to meet other learners and improve your listening and speaking skills as well as learning about each others cultures for FREE!
          </p>
        </div>

        <div class="tile is-ancestor">
          <div class="tile is-parent">
            <article class="tile is-child box">
              <p class="title">
                Join Slack >>
              </p>
              <p class="subtitle">
              </p>
            </article>
          </div>
          <div class="tile is-parent">
            <article class="tile is-child box">
              <p class="title">
                Meet Others >
              </p>
              <p class="subtitle">
              </p>
            </article>
          </div>
          <div class="tile is-parent">
            <article class="tile is-child box">
              <p class="title">
                Learn More !
              </p>
              <p class="subtitle">
              </p>
            </article>
          </div>
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
      title: `About | ${this.$siteConfig.siteName}`
    }
  },
  components: { QuoteCard }
}
</script>
