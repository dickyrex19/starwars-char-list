<template>
  <div class="people">
    <h1>List Characters</h1>
    <div class="wrapper" v-for="item in items">
      <div class="card">
        {{ item.name }}
      </div>
    </div>
  </div>
</template>

<style>
@media (min-width: 768px) {
  h1 {
    font-size: 3rem;
  }
  .wrapper {
    display: flex;
  }
  .card {
    margin: 5px;
    border: 1px solid #fff;
    padding: 10px 40px;
    width: 100%;
  }
}
</style>

<script>
export default {
  data() {
    return {
      items: [
        { name: "Luke Skywalker" },
        { name: "C-3PO" },
        { name: "R2-D2" },
        { name: "Darth Vader" },
        { name: "Leia Organa" },
        { name: "Owen Lars" },
        { name: "Beru Whitesun lars" },
        { name: "R5-D4" },
        { name: "Biggs Darklighter" },
        { name: "Obi-Wan Kenobi" },
      ],
    };
  },
};
</script>
