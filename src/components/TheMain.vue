<template>
  <div>
    <JumbotronContent></JumbotronContent>
    <MarketingSection></MarketingSection>
    <TipsSection></TipsSection>
    <PopularFeatures></PopularFeatures>
    <TestimonialsSection></TestimonialsSection>
  </div>
</template>

<script>
import MarketingSection from './MarketingSection.vue';
import JumbotronContent from './JumbotronContent.vue';
import TipsSection from './TipsSection.vue';
import PopularFeatures from './PopularFeatures.vue';
import TestimonialsSection from './TestimonialsSection.vue';
export default {
    components: { MarketingSection, JumbotronContent, TipsSection, PopularFeatures, TestimonialsSection }
}
</script>

<style>

</style>