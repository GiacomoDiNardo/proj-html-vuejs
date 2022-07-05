<template>
  <div>
    <JumbotronContent></JumbotronContent>
    <MarketingSection></MarketingSection>
    <TipsSection></TipsSection>
    <PopularFeatures></PopularFeatures>
    <TestimonialsSection></TestimonialsSection>
    <LatestPostSection></LatestPostSection>
    <ContactsSection></ContactsSection>
  </div>
</template>

<script>
import MarketingSection from './MarketingSection.vue';
import JumbotronContent from './JumbotronContent.vue';
import TipsSection from './TipsSection.vue';
import PopularFeatures from './PopularFeatures.vue';
import TestimonialsSection from './TestimonialsSection.vue';
import LatestPostSection from './LatestPostSection.vue';
import ContactsSection from './ContactsSection.vue';
export default {
    components: { MarketingSection, JumbotronContent, TipsSection, PopularFeatures, TestimonialsSection, LatestPostSection, ContactsSection }
}
</script>

<style>

</style>