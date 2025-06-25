<script setup>
definePageMeta({
  layout: "landing",
});

var gtmTag = `
<!-- Google tag (gtag.js) -->
<script async src="https://www.googletagmanager.com/gtag/js?id=G-Y9BM7XHFYW">
<\/script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());

  gtag('config', 'G-Y9BM7XHFYW');
<\/script>
`;
useHead({ script: gtmTag });
</script>

<template>
  <LandingContainer>
    <LandingHero></LandingHero>
    <LandingFeatures></LandingFeatures>
    <LandingLogos></LandingLogos>
    <LandingCta></LandingCta>
  </LandingContainer>
</template>
