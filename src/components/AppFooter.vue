<template>
  <footer class="d-flex">
    <div class="footer-column" v-for="(column, index) in footerData" :key="index">
      <h4>{{ column.title }}</h4>
      <ul>
        <li v-for="(item, idx) in column.items" :key="idx">{{ item }}</li>
      </ul>
    </div>
  </footer>
</template>

<script>
export default {
  data() {
    return {
      footerData: [
        { title: 'Colonna 1', items: ['Link 1', 'Link 2', 'Link 3'] },
        { title: 'Colonna 2', items: ['Link 4', 'Link 5', 'Link 6'] },
        { title: 'Colonna 3', items: ['Link 7', 'Link 8', 'Link 9'] },
        { title: 'Colonna 4', items: ['Link 10', 'Link 11', 'Link 12'] },
      ],
    };
  },
};
</script>

<style scoped>
footer {
  background-color: #e9ecef;
  padding: 40px;
  display: flex;
  justify-content: space-between;
}
  .footer-column {
    width: 25%;
  }
    ul {
      list-style-type: none;
      padding: 0;
    }
      li {
        padding: 5px 0;
      }
   
</style>
