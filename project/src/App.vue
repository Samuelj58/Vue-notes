<template>
  <div>
      <h1>Buy your consoles here!!</h1>
      <ul>
          <li v-for="(console, index) in consoles" :key="index">
              {{ console.name }} - Price: ${{ console.price }} - Available: {{ console.available ? 'Yes' : 'No' }}
          </li>
      </ul>
  </div>
</template>

<script>
export default {
  data() {
      return {
          consoles: [
              {
                  name: 'PlayStation 5',
                  price: 449.99,
                  Controller: true,
                  img: "https://media.gamestop.com/i/gamestop/11108141?$pdp2x$"
              },
              {
                  name: 'Xbox',
                  price: 449.99,
                  Controller: true,
                  img: "https://media.gamestop.com/i/gamestop/11108371?$pdp2x$"
              },
              {
                  name: 'Nintendo Switch',
                  price: 259.99,
                  Controller: true,
                  img: "https://media.gamestop.com/i/gamestop/11095819?$pdp2x$"
              },
              {
                  name: 'Steam Deck',
                  price: 278.99,
                  Controller: true,
                  img: "https://media.gamestop.com/i/gamestop/20003488-1?$pdp2x$"
              },
              {
                  name: 'ROG ally',
                  price: 888.99,
                  Controller: true,
                  img: "https://www.zoro.com/static/cms/product/large/DH%20Commerce%20dba%20Streamline%20Distributors_6542964cv16dxxxx1xxxx788028.jpeg"
              }
          ]
      };
  }
};


</script>

<style lang="scss" scoped>

</style>
