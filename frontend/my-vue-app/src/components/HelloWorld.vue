<template>
  <div class="hello">
    <h1>Data from Neo4j:</h1>
    <ul v-if="data">
      <li v-for="(item, index) in data" :key="index">{{ item }}</li>
    </ul>
    <p v-else>Loading...</p>
  </div>
</template>

<script>
import axios from 'axios';

export default {
  name: 'HelloWorld',
  data() {
    return {
      data: null
    };
  },
  created() {
    this.fetchData();
  },
  methods: {
    fetchData() {
      axios.get('http://localhost:5000/data')
        .then(response => {
          this.data = response.data;
        })
        .catch(error => {
          console.error('There was an error fetching the data:', error);
        });
    }
  }
};
</script>