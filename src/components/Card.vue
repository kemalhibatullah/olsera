<template>
  <el-card
    v-for="o in 5"
    :key="o"
    class="text item"
    style="
    margin-bottom: 30px;
    margin-left: 30px;
    margin-right: 30px; 
      display: flex;
      justify-content: space-between;"
  >
    <div>{{ "List item " + o }}</div>
    <div>icon
    {{info}}</div>
  </el-card>
</template>

<script>
import axios from 'axios';

export default {
    mounted () {
    axios
      .get('https://jsonplaceholder.typicode.com/posts?_page=1&_limit=5')
      .then(response => (this.info = response))
  }
}
</script>
