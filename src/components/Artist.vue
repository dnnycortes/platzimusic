<template lang="pug">
    li 
        h2: a( v-bind:href="artist.url" target="_blank" ) {{ artist.name }}
        img( v-bind:src="artist.image[2]['#text']" )
</template>

<script>
export default {
  name: 'artist', // nombre del componente
  props: ['artist'] // propiedades que recibe
}
</script>

<style lang="stylus" scoped>
li 
    display block 
    margin 10px 0
</style>
