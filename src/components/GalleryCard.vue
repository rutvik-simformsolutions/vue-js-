<template>
  <div class="card" style="width: 18rem">
    <img class="card-img-top" alt="Car-image" src="@/assets/tesla-model-x.jpg" />
    <div class="card-body">
      <h5 class="card-title">{{ modelName }}</h5>
      <div class="card-text m-3">
        <table>
          <tr>
            <th>Range :</th>
            <td>{{ range }}</td>
          </tr>
          <tr>
            <th>Power :</th>
            <td>{{ power }}</td>
          </tr>
          <tr>
            <th>Weight :</th>
            <td>{{ weight }}</td>
          </tr>
          <tr>
            <th>Seating :</th>
            <td>{{ seating }}</td>
          </tr>
        </table>
      </div>
      <a v-on:click="showPrice()" href="#" class="btn btn-primary">info</a>
    </div>
  </div>
</template>

<script>
export default {
  name: "GalleryCard",
  data() {
    return {
      modelName: "Tesla Model-X",
      imageurl: "/assets/tesla-model-x.jpg",
      range: "333 mi",
      power: "1020 hp",
      weight: "5,000 lbs",
      seating: "Up to 7",
    };
  },
  methods: {
    showPrice() {
      alert("$112,590*");
    },
  },
};
</script>

<style>
td th {
  text-align: justify !important;
}
</style>
