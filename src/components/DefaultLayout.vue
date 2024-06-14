<template>
   <navbar/>
 
    
    <main>
      <div class="max-w-[1200px] max-auto">
      <router-view />
    </div>
    </main>

</template>

<script setup>
import Navbar from "./Navbar.vue";
</script>
