<script setup>
import doug from "@/components/doug.vue";
import wren from "@/components/wren.vue";
import dougpfp from "@/components/dougpfp.vue";
import pepperpfp from "@/components/pepperpfp.vue";
</script>
<template>
  <div class="bio">
      <dougpfp></dougpfp>
      <wren ></wren>
      <pepperpfp />
    <doug />
  </div>
</template>

<style>
    .bio {
        display:grid;
        grid-template-columns: auto 1fr;
        grid-template-rows: auto auto auto auto;
        grid-gap:15px
    }
    .dougpfp {
        grid-column: 1;
        grid-row: 1 / span 2;
    }
    .wren {
        grid-row: 1;
        grid-column: 2;
    }
    .wren2 {
        grid-row:2;
        grid-column:2;
    }
    .pepperpfp{
               grid-column: 1;
        grid-row: 3 / span 2;
    }
    .pogpepper{
       grid-row:3;
        grid-column:2; 
    }
    .pogpepper2 {
        grid-row:4;
        grid-column:2;
        margin-bottom: 50px;
    }

</style>
