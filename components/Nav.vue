<template>
    <div>
        <nav class="navbar navbar-expand-lg navbar-dark bg-dark">
  <div class="container-fluid">
    <a class="navbar-brand" href="/">Restuarants Directory</a>
    
    <div class="collapse navbar-collapse " id="navbarSupportedContent">
      <ul class="navbar-nav ml-auto mb-2 mb-lg-0 ">
        <li class="nav-item">
          <nuxt-link to="/" class="nav-link active" aria-current="page" >Home</nuxt-link>
        </li>
        <li class="nav-item">
         
          <nuxt-link to="/restuarants" class="nav-link active" aria-current="page" >Restuarants</nuxt-link>
        </li>
    
      </ul>
     
    </div>
  </div>
</nav>
    </div>
</template>
<style >
.ml-auto{
    margin-left: auto;
}
</style>