<template>
  <div class="contactBox">
    <ContactForm></ContactForm>
    <Map></Map>
  </div>
</template>

<script>
import ContactForm from "@/components/ContactForm.vue";
import Map from "@/components/Map.vue";
export default { components: { ContactForm, Map } };
</script>

<style scoped>
.contactBox {
  display: grid;
  grid-template-columns: 0.7fr 1fr;
}
</style>