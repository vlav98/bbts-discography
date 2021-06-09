<template>
  <router-link to="/home" class="px-3 py-2 rounded-md text-sm font-medium text-white bg-gray-900">Home</router-link>

  <router-link to="/about" class="px-3 py-2 rounded-md text-sm font-medium text-white hover:text-white hover:bg-gray-700">About</router-link>

  <router-link to="/contact" class="px-3 py-2 rounded-md text-sm font-medium text-white hover:text-white hover:bg-gray-700">Contact</router-link>
</template>

<script>
export default {
  name: "NavBar",
  components: {},
};
</script>
