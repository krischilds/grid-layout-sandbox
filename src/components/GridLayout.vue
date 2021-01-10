<template>
  <div class="grid-layout">
    <header class="header">Notes Application</header>
    <nav class="nav">This is nav links</nav>
    <section class="note-form">Note Form</section>
    <section class="notes-view">Notes View</section>
    <section class="note-view">Note View</section>
  </div>
</template>

<script>
export default {
  name: "GridLayout",
  props: {
    msg: String,
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="scss" scoped>
.grid-layout {
  display: grid;
  grid-template-columns: minmax(300px, 1fr) repeat(4, minmax(100px, 1fr));
  grid-template-rows: minmax(20px, 0.25fr) 0.25fr minmax(200px, 2fr) minmax(
      200px,
      1fr
    );
  grid-gap: 1px;
  margin: 0;
  padding: 0;
  border: 0;

  width: 100vw;
  height: 100vh;

  background: orange;

  .header {
    background: lightcoral;
    grid-column: span 5;
  }

  .nav {
    background: lightgreen;
    grid-column: span 5;
  }

  .notes-view {
    grid-column: span 3;
  }

  .note-view {
    background: lightblue;
    grid-column: span 5;
  }

  .note-form {
    background: lightYellow;
    grid-column: minmax(300px, 1fr);
  }
}
</style>
