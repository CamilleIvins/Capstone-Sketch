<template>
  <!-- <style>
    main.debug .container,
    main.debug .container-fluid {
      outline: 2px double blue;
      outline-offset: -2px;
    }

    main.debug .row {
      outline: 2px dashed red;
      outline-offset: -2px;
    }

    main.debug [class*="col-"] {
      outline: 2px dotted forestgreen;
      outline-offset: -3px;
    }
  </style> -->
  <!-- <div class="home flex-grow-1 d-flex flex-column align-items-center justify-content-center">
    <div class="home-card p-5 bg-white rounded elevation-3">
      <img src="https://bcw.blob.core.windows.net/public/img/8600856373152463" alt="CodeWorks Logo"
        class="rounded-circle">
      <h1 class="my-5 bg-dark text-white p-3 rounded text-center">
        Vue 3 Starter
      </h1>
    </div>
  </div> -->


  <section class="container-fluid bg-img">
    <!-- logo and map that routes to map page -->
   
      <section class="row justify-content-around">
        <div class="col-5">
          LOGO

        </div>
        <div class="col-6">
          Map/link to map page

        </div>
      </section>
<!-- photo and stache chart with links to popular staches -->
      <section class="row justify-content-around">

        <div class="col-6">
         Generic Pic

        </div>
        <div class="col-5">
          Stache chart

        </div>
      </section>
  </section>
</template>

<script>
export default {
  setup() {
    return {}
  }
}
</script>

<style scoped lang="scss">
.home {
  display: grid;
  height: 80vh;
  place-content: center;
  text-align: center;
  user-select: none;

  .home-card {
    width: 50vw;

    >img {
      height: 200px;
      max-width: 200px;
      width: 100%;
      object-fit: contain;
      object-position: center;
    }
  }
}

.container,.container-fluid {
      outline: 2px double blue;
      outline-offset: -2px;
    }

   .row {
      outline: 2px dashed red;
      outline-offset: -2px;
    }

    [class*="col-"] {
      outline: 2px dotted forestgreen;
      outline-offset: -3px;}

      .bg-img {
  // Uncomment after change text color
  background-image: url(../assets/img/Geo-Stache-logo.png);
height: 20vh;
 
 
}
</style>
