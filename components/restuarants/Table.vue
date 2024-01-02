<template>
  <div class="table">
    <h1>TOP 50: THE RANKING</h1>
    <div class="table-container">
      <div class="table-col">
        <RestuarantsRow  :isHeader="true" />
        <RestuarantsRow  v-for="(res,index) in restuarantsOrganized.first" 
       :key="res.id"
       :name="res.name"
       :rank="res.rank"
       :index="index"
       />
      </div>
      <div class="table-col">
        <RestuarantsRow  :isHeader="true" />
        <RestuarantsRow  v-for="(res,index) in restuarantsOrganized.second" 
       :key="res.id"
       :name="res.name"
       :rank="res.rank"
       :index="index"
       />
      </div>
    </div>
  </div>
</template>
<script setup lang="ts">
import restuarants from "@/data.json"
const restuarantsOrganized ={
first: [...restuarants].splice(0,25),
second:[...restuarants].splice(25,25)
}
</script>

<style scoped>
.table {
  margin: 3rem 0;
}
.table h1 {
  margin-bottom: 2rem;
}
.table-container {
  display: flex;
  justify-content: space-between;
}
.table-col {
  width: 48%;
}
</style>