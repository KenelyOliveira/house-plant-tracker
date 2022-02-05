<template>
  <div class="container">
    <br />
    <Header />
    <br />
    <br />
    <br />
    <div>
      <router-link to="/" tag="button" class="btn btn-primary active">Search</router-link>
    </div>
    <div>
      <router-link to="/new-plant" tag="button" class="btn btn-success active">Add new plant</router-link>
    </div>
    <div>
      <button class="btn btn-success active">Add progress</button>
    </div>
  </div>
</template>

<script lang="ts">
import Header from '@/components/Header.vue';
import { Options, Vue } from 'vue-class-component';

@Options({
  components: {
    Header
  },
})
export default class Home extends Vue {


}
</script>

<style scoped>
.btn {
  width: 300px;
}
div {
  padding-bottom: 20px;
}
</style>