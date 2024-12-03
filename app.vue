<template>
  <div>
    <NuxtLayout>
      <NuxtPage />
    </NuxtLayout>
  </div>
</template>

<script setup lang="ts">
useSchemaOrg([
  defineOrganization({
    "@type": "MedicalOrganization",
    address: {
      addressCountry: "AT",
      addressLocality: "Wien",
      addressRegion: "Wien",
      postalCode: "1234",
      streetAddress: "Musterstrasse 1234",
    },
    description: "Description",
    isAcceptingNewPatients: true,
    logo: "https://upload.wikimedia.org/wikipedia/commons/9/9c/Dunder_Mifflin%2C_Inc.svg",
    medicalSpecialty: "http://schema.org/PrimaryCare",
    name: "ACME Corp",
    sameAs: [
      "https://example.com",
    ],
    slogan: "Limitless Paper in a Paperless World",
  }),
  defineWebSite({
    name: "ACME Corp",
  }),
  defineWebPage(),
]);
</script>

