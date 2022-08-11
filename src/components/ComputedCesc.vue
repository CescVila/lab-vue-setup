<template>
<div id="computed-part-one">
  <h1>Guitarrist - {{firstName}} {{lastName}}</h1>
  <h1>Computed Property - Guitarrist {{favGuitarrist}}</h1>

  <button @click="changeFavGuitarrist">Change Favorite Guitarrist</button>
</div>





<div>
  <h1>Using computed method</h1>
  <template v-for="(item, index) in computedItemList" :key="index">
    <h1>{{item.title}} - {{item.price}}</h1>
  </template>
</div>

</template>

<script>
export default {
  data() {
    return {
      firstName: "Gustavo",
      lastName: "Cerati Martinez",
      items: [
        {title:"screen", price: 100},
        {title:"earphone", price: 30},
        {title:"chair", price: 150},
        {title:"mouse", price: 20 },
        {title:"coffe cup", price: 5},
        ]
    };
  },
  methods: {
    changeFavGuitarrist() {
      this.favGuitarrist2= "Cesc Vila"
    },
  },
  computed: {
    favGuitarrist(){
      return `${this.firstName} ${this.lastName}`;
    },
    favGuitarrist2: {
      get() {
      return `${this.firstName} ${this.lastName}`;
      },
      set(value) {
        const name = value.split(" ");
        this.firstName = name[0];
        this.lastName =name [1];
      },
    },
   computedItemList() {
    return this.items.filter((item) => item.price < 100);
   },
  },
};
</script>

<style>

</style>