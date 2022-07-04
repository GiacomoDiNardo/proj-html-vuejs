<template>
  <div>
    <JumbotronContent></JumbotronContent>
    <MarketingSection></MarketingSection>
    <TipsSection></TipsSection>
    <PopularFeatures></PopularFeatures>
  </div>
</template>

<script>
import MarketingSection from './MarketingSection.vue';
import JumbotronContent from './JumbotronContent.vue';
import TipsSection from './TipsSection.vue';
import PopularFeatures from './PopularFeatures.vue';
export default {
    components: { MarketingSection, JumbotronContent, TipsSection, PopularFeatures }
}
</script>

<style>

</style>