<script setup>
const features = [
  {
    title: "SEO Enabled",
    description:
      "Automatic sitemaps, RSS feeds, pagination and collections take the pain out of SEO and syndication. It just works!",
    icon: "bx:bxs-file-find",
  },
  {
    title: "Cheap pay-as-you-sell plans",
    description:
      "We can charge a small fee on your products sold to test the waters before going big. No large up front payments required",
    icon: "bx:bxs-briefcase",
  },
  {
    title: "Social Media and Mobile",
    description:
      "We can help with social media advertising, product placement and build our sites 'mobile first' so that they work on all platforms",
    icon: "bx:bxs-bot",
  },
];
</script>

<template>
  <div class="mt-16 md:mt-0">
    <h2 class="text-4xl lg:text-5xl font-bold lg:tracking-tight">
      Everything you need to start a website
    </h2>
    <p class="text-lg mt-4 text-slate-600">
      We take you from "Where do I even start?" to generating passive income
      through product and service sales on your website.
    </p>
  </div>

  <div class="grid sm:grid-cols-2 md:grid-cols-3 mt-16 gap-16">
    <div v-for="item of features" class="flex gap-4 items-start">
      <div class="mt-1 bg-black rounded-full p-2 w-8 h-8 shrink-0">
        <Icon class="text-white" :name="item.icon" />
      </div>
      <div>
        <h3 class="font-semibold text-lg">{{ item.title }}</h3>
        <p class="text-slate-500 mt-2 leading-relaxed">
          {{ item.description }}
        </p>
      </div>
    </div>
  </div>
</template>
