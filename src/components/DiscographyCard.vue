<template>
  <div class="rounded border border-black flex justify-between bg-primary dark">
    <h3>{{ discographyData.Name }}</h3>
    <p><span style="font-weight: bold">Genre</span> : {{ discographyData.Genre }}</p>
    <div class="flex">
      <base-button class="add mr-2" :backgroun="bg - secondary" title="Add One" :index="index" @click="addData(discographyData)" />
      <base-button class="remove" :background="bg - danger" title="Remove One" :index="index" @click="removeData(discographyData)" />
    </div>
    <div class="bg-gradient-to-br from-fuchsia-500 to-purple-600"></div>
    <!--
    <div class="bg-gradient-to-br from-light-blue-400 to-indigo-500"></div>
    -->
    <!--
    <div class="bg-gradient-to-br from-cyan-400 to-light-blue-500"></div>
    -->
    <!--
    <div class="bg-gradient-to-br from-green-400 to-cyan-500"></div>
    -->
    <!--
    <div class="bg-gradient-to-br from-yellow-400 to-orange-500"></div>
    -->
    <!--
    <div class="bg-gradient-to-br from-pink-500 to-rose-500"></div>
    -->
  </div>
</template>

<script>
export default {
  name: "main-view",
  props: {
    discographyData: Object,
    index: Number,
    clickMethod: Function,
  },
  methods: {
    addData: function (discography) {
      this.$emit("add-data", discography);
    },
    removeData: function (discography) {
      this.$emit("remove-data", discography);
    },
  },
  computed: {},
};
</script>

<style></style>
