<template>
  <div>
    <hero />
    <features />
    <team />
    <teasers />
    <prices />
    <call-to-action />
  </div>
</template>

<script>
import Hero from '@/components/Hero'
import Team from '@/components/Team'
import Features from '@/components/Features'
import Teasers from '@/components/Teasers'
import Prices from '@/components/Prices'
import CallToAction from '@/components/CallToAction'
export default {
  name: 'LandingPage',
  components: {
    hero: Hero,
    team: Team,
    features: Features,
    teasers: Teasers,
    prices: Prices,
    'call-to-action': CallToAction
  }
}
</script>