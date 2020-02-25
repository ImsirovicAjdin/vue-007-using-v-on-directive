<template>
  <div class="hello">
    <!-- 'whatIsVue' and 'whyUseVue' are functions defined in the 'methods' option in the Vue instance -->
    <button id="btn" v-on:click="whatIsVue()">What is Vue?</button>
    <button id="btn" v-on:click="whyUseVue()">Why use Vue?</button>
  </div>
</template>

<script>
export default {
  name: "HelloWorld",
  data() {
    return {
      name: "Vue.js"
    };
  },
  methods: {
    whatIsVue: function() {
      console.info(this.name + " is a Progressive Front-end Framework");
    },
    whyUseVue: function() {
      alert("Because " + this.name + " is nice.");
    }
  }
};
</script>
