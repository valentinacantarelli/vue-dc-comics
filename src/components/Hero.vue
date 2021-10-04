<template>
  <div class="hero" :style="`background-image:url(${bgImg})`"></div>
</template>

<script>
export default {
    name:"Hero",
    props:["bgImg"]
}
</script>

<style lang="scss" scope>
.hero{
    height:250px;
    background-repeat: no-repeat;
    background-size: cover;
}
</style>