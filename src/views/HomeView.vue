<template>
  <div class="home">Home</div>
</template>

<script>
export default {
  name: "HomeView",
  methods: {
    async fetchCovidData() {
      const res = await fetch("https://api.covid19api.com/summary");
      const data = await res.json();
      return data;
    },
  },
  created() {
    const data = this.fetchCovidData();
    console.log(data);
  },
};
</script>
