<template>
  <dir>
    <header>
      <div class="row">
        <div class="col col-sm-12">
          <h1>Site</h1>
          <app-cart></app-cart>  
        </div>
      </div>
    </header>
    <section>
      <div class="container">
        <div class="row">
          <div class="col col-sm-12">
            <app-product></app-product>
          </div>
        </div>
      </div>
    </section>
  </dir>
</template>

<script>
  import AppProduct from './components/Product';
  import AppCard from './components/Card';

export default {
  components: {
    AppProduct,
    AppCard
  }
}
</script>

<style>

</style>
