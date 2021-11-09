<template>
  <ul class="auto-grid">
    <li>Item 1</li>
    <li>Item 2</li>
    <li>Item 3</li>
    <li>Item 4</li>
    <li>Item 5</li>
    <li>Item 6</li>
    <li>Item 7</li>
    <li>Item 8</li>
    <li>Item 9</li>
    <li>Item 10</li>
    <li>Item 11</li>
    <li>Item 12</li>
  </ul>
</template>

<script>
export default {
  layout(context) {
    return "blog";
  },
};
</script>

 <style>
/*
  AUTO GRID
  Set the minimum item size with `--auto-grid-min-size` and you'll
  get a fully responsive grid with no media queries.
*/
.auto-grid {
  --auto-grid-min-size: 20rem;

  display: grid;
  grid-template-columns: repeat(
    auto-fill,
    minmax(var(--auto-grid-min-size), 1fr)
  );
  grid-gap: 1rem;
}

/* Presentational styles */

body {
  background: #efefef;
  padding: 1rem;
  line-height: 1.4;
  font-family: sans-serif;
}

li {
  padding: 5rem 1rem;
  text-align: center;
  font-size: 1.2rem;
  background: snow;
  border-left: 15px inset blue;
  border-radius: 5px;
  color: #ffffff;
}
</style>
