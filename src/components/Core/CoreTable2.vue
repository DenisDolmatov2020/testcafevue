<script setup lang="ts">

</script>

<template>
  <table class="container">
    <thead>
    <tr>
      <th><h1>Sites</h1></th>
      <th><h1>Views</h1></th>
      <th><h1>Clicks</h1></th>
      <th><h1>Average</h1></th>
    </tr>
    </thead>
    <tbody>
    <tr>
      <td>Google</td>
      <td>9518</td>
      <td>6369</td>
      <td>01:32:50</td>
    </tr>
    <tr>
      <td>Twitter</td>
      <td>7326</td>
      <td>10437</td>
      <td>00:51:22</td>
    </tr>
    <tr>
      <td>Amazon</td>
      <td>4162</td>
      <td>5327</td>
      <td>00:24:34</td>
    </tr>
    <tr>
      <td>LinkedIn</td>
      <td>3654</td>
      <td>2961</td>
      <td>00:12:10</td>
    </tr>
    <tr>
      <td>CodePen</td>
      <td>2002</td>
      <td>4135</td>
      <td>00:46:19</td>
    </tr>
    <tr>
      <td>GitHub</td>
      <td>4623</td>
      <td>3486</td>
      <td>00:31:52</td>
    </tr>
    </tbody>
  </table>
</template>

<style scoped lang="scss">

.blue { color: #0ea4e8; }
.yellow { color: #FFF842; }

.container td {
  font-weight: normal;
  font-size: 1em;
  -webkit-box-shadow: 0 2px 2px -2px #dcdee3;
  -moz-box-shadow: 0 2px 2px -2px #d5d6d7;
  box-shadow: 0 2px 2px -2px #c9cace;
}

.container {
  text-align: left;
  overflow: hidden;
  width: 80%;
  margin: 0 auto;
  display: table;
  padding: 0 0 8em 0;
  font-weight: 700;
}

.container td, .container th {
  padding-bottom: 2%;
  padding-top: 2%;
  padding-left:2%;
}

/* Background-color of the odd rows */
.container tr:nth-child(odd) {
  background-color: #d0d2d5;
}

/* Background-color of the even rows */
.container tr:nth-child(even) {
  background-color: #2C3446;
  color: #E5E7EB;
}

.container th {
  color: #E5E7EB;
  background-color: #1F2739;
}

.container td:first-child { color: #FB667A; }

.container tr:hover {
  background-color: #464A52;
  -webkit-box-shadow: 0 6px 6px -6px #0E1119;
  -moz-box-shadow: 0 6px 6px -6px #0E1119;
  box-shadow: 0 6px 6px -6px #0E1119;
}

.container td:hover {
  background-color: #FFF842;
  color: #403E10;
  font-weight: bold;
  box-shadow: #7F7C21 -1px 1px, #7F7C21 -2px 2px, #7F7C21 -3px 3px, #7F7C21 -4px 4px, #7F7C21 -5px 5px, #7F7C21 -6px 6px;
  transform: translate3d(6px, -6px, 0);

  transition-delay: 0s;
  transition-duration: 0.4s;
  transition-property: all;
  transition-timing-function: line;
}

@media (max-width: 800px) {
  .container td:nth-child(4),
  .container th:nth-child(4) { display: none; }
}
</style>
