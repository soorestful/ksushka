<script setup>
import { RouterLink, RouterView } from 'vue-router'

</script>

<template>
  <div id="everything">
      <nav id="rlinks">
        <RouterLink to="/" class="rlink" id="homelink">First page</RouterLink>
        <RouterLink to="/about" class="rlink">Second page</RouterLink>
      </nav>
  <main>
  <RouterView />
  </main>
  </div>
</template>

<style scoped>
#everything{
  width:100vh;
  height:100vh;
  display:flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  margin:0;
}
#rlinks{
  width:100%;
  margin-top: 20%;
  display: flex;
  flex-direction: row;
  align-items: center;
  justify-content: center;
}
.rlink{
  background-color:white;
  padding:1% 2% 1% 2%;
  border-radius: 20px;
  color:rgb(85, 98, 110);
  text-decoration: none;
}
.rlink:visited{
  color:rgb(85, 98, 110);
  text-decoration: none;
}
#homelink{
  margin-right: 5%;
}
</style>
