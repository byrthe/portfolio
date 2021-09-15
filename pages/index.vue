<template>
   <div>
       <Getlost />
       <Skillbank />
       <Delhaize />
       <Tri />
       <Posters />
       <Krisis />
       <Sotu />
       <!-- <Bday /> -->
    </div>
</template>

<script>
export default {
  lazyComponents: [
    'Getlost',
    'Skillbank',
    'Tri',
  ],
}
</script>
