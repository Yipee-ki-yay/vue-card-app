<template>
    <header>
      <div class="container">
        <div class="row">
          <div class="col col-sm-12">
            <h1>Site</h1>
            <app-card></app-card>  
          </div>
        </div>
      </div>
    </header> 
</template>

<script>
    import AppCard from './Card';

    export default {
        components: {
            AppCard
        }
    }
</script>


