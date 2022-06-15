<template>
  <div class="spin">

  </div>
</template>

<script>
export default {

}
</script>

<style scoped>
    .spin{
        display: block;
        width: 40px;
        margin: 30px auto;
        height: 40px;
        border: solid 3px transparent; 
        border-radius: 50px;
        border-top-color: #ff8800;
        animation: spin 0.5s ease infinite;
    }
    @keyframes spin{
        to{
            transform: rotateZ(360deg)
        }
    }
</style>