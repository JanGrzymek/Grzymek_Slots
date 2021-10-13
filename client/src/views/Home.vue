<template>
  <div>
    <AppLayout>
      <template v-slot:header> I was made with Vue slots! </template>
      <AppButton><img src="../../public/images/home.svg" /> Home</AppButton>
      <template v-slot:footer> By Robert Baumgartner </template>
    </AppLayout>
  </div>
</template>

<script>
// @ is an alias to /src
import AppLayout from "@/components/AppLayout.vue";

export default {
  name: "Home",
  components: {
    AppLayout,
  },
};
</script>
