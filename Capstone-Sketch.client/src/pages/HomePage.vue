<template>

  <section class="container">
    <!-- <img src="../assets/img/Geo-Stache-logo.png" style="height: 800px;" alt=""> -->
    <!-- logo and map that routes to map page -->
   
      <section class="row justify-md-content-around justify-content-center my-1">
        <div class="col-md-5 col-4 order-md-0 order-1">
          <img class="logo" src="../assets/img/GeoStache.png" alt="">

        </div>
        <div class="col-md-7 col-12 position-relative p-0 my-md-0 my-2 map-link order-md-1 order-0">
          <!-- Map/link to map page -->
          <img class="map-pic" src="https://c1.wallpaperflare.com/preview/97/283/810/boise-idaho-overhead-view-public-domain.jpg" alt="">
          <div class="frosted-card">
            <h1 class="ps-2 position-relative">Start searching</h1>
          </div>
        </div>
      </section>
<!-- photo and stache chart with links to popular staches -->
<div class="row justify-content-center">
  <button class="btn create my-3 col-8 col-md-4 fs-3">
    Post a Stache
  </button>
</div>
      <section class="row justify-content-around my-2">

        <div class="col-md-6 col-12 p-0">
          <img class="homepage-pic px-0" src="https://assets.simpleviewinc.com/simpleview/image/upload/c_limit,h_1200,q_75,w_1200/v1/clients/topeka/Geocache_Lego_guy_ab282473-4f3c-43cf-ad96-5b676481fb3c.jpg" alt="">
        </div>

        <div class="col-md-5 col-12 glass-card my-md-0 my-2">
          <table class="row">
  <tr class="col-8">
    <th class="col-2 px-1">Company</th>
    <th class="col-7 px-1">Contact</th>
    <th class="col-3 px-1">Country</th>
  </tr>
  <tr>
    <td class="col-2 px-1">Alfreds Futterkiste</td>
    <td class="col-7 px-1">Maria Anders</td>
    <td class="col-3 px-1">Germany</td>
  </tr>
  <tr>
    <td class="col-2 px-1">Centro comercial Moctezuma</td>
    <td class="col-7 px-1">Francisco Chang</td>
    <td class="col-3 px-1">Mexico</td>
  </tr>
</table>

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
// show up on this size and smaller
@media screen and (max-width: 768px) {
.logo{
  margin-top: 1em;
  margin-bottom: 1em;
}

.map-link{
  img{
  width: 100%;
  height: 70vh !important;
  border-radius: 10px;
  object-fit: cover;
object-position: center;
border-radius: 0px !important;
}

box-shadow: 0 3px 3px -1px rgba(43, 43, 43, 0.85), 
  0 5px 6px 0 rgba(43, 43, 43, 0.79), 
  0 1px 8px 0 rgba(43, 43, 43, 0.79);
}
.map-link:hover{
transform: scale(1) !important;
transition: ease .35s;
filter: brightness(1.2);
}
}
.logo{
  max-width: 100%;
  // filter:drop-shadow (0 0 0.75rem crimson)
  filter: drop-shadow(3px 8px 7px #292828);
}
.map-link{
  img{
  width: 100%;
  height: 100%;
  border-radius: 10px;
  object-fit: cover;
object-position: center;
border-radius: 10px;
}

box-shadow: 0 3px 3px -1px rgba(43, 43, 43, 0.85), 
  0 5px 6px 0 rgba(43, 43, 43, 0.79), 
  0 1px 8px 0 rgba(43, 43, 43, 0.79);
}
.map-link:hover{
  border-radius: 10px;

transform: scale(1.03);
transition: ease .35s;
box-shadow: 0 0 10px 3px rgba(205, 205, 205, 0.85),
inset 0 0 5px 5px rgba(205, 205, 205, 1);
  // 0 5px 6px 0 rgba(205, 205, 205, 0.79)
  overflow-x: clip;
}

.frosted-card{
  backdrop-filter: blur(5px);
    background-color: rgba(219, 220, 221, 0.592);
    border-top-left-radius: 5px;
    border-top-right-radius: 5px;
    top: 0;
    position: absolute;
    width: 100%;
}
// .frosted-card:hover{
//   backdrop-filter: blur(5px);
//     background-color: rgba(219, 220, 221, 0.592);
//     border-top-left-radius: 5px;
//     border-top-right-radius: 5px;
//     top: 0;
//     position: absolute;
//     width: 100%;
//     transform: scale(1.03);
// transition: ease .35s;
// }

.homepage-pic{
  border-radius: 10px;
  width: 100%;
  object-fit: cover;
object-position: center;
box-shadow: 0 3px 3px -1px rgba(43, 43, 43, 0.85), 
  0 5px 6px 0 rgba(43, 43, 43, 0.79), 
  0 1px 8px 0 rgba(43, 43, 43, 0.79);
}

.glass-card{
  border-radius: 10px;
  backdrop-filter: blur(3px);
  background-color: rgba(245, 245, 245, 0.432);
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

  button.create{
    background-color: #fe9030;
  }
  button.create:hover{
    background-color: rgb(254, 144, 48);
    box-shadow: 0 0 10px 2px rgb(254, 144, 48);
  }


//       img {
//   // Uncomment after change text color
//   background-image: url(/assets/img/Geo-Stache-logo.png);
//   object-fit: contain;
//   object-position: center;
//   max-height: 800px;
 
 
// }
</style>
