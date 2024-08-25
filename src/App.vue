<template>
  <div>
    <h1 class="title">{{ism}}</h1>
    <h1>{{count}}</h1>
    <h1>{{fullname}}</h1>
    <button @click="plus()">plus</button>
    <button @click="minus()">Minus</button>
  </div>
</template>

<script>
// import BaseBtnVue from './components/BaseBtn.vue';
  export default {
    data() {
      return {
        ism: 'ghostjon pubg please subcribes',
        fam: 'My name is Dior',
        count: 0
      }
    },
    methods: {
      plus() {
        this.count++
      },
      minus(){
        this.count--
      }
    },
    computed: {
      fullname() {
        return this.ism + this.fam 
      }
    },
  }
</script>

<style scoped>

</style>
