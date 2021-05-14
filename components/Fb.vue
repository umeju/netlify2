<template>

  <a
    href="fb://facewebmodal/f?href=https://www.facebook.com/www.hubanero.it"
  >
    <div class="FbLogo loghi"></div>

  </a>
</template>


<script>
export default {
  data() {
    return {

      url: "fb://facewebmodal/f?href=https://www.facebook.com/www.hubanero.it"
    }
  }
}
</script>


<style scope>
.FbLogo {
  background-image: url(/fb.png);
}
@keyframes appear {
  0% {
    opacity: 0;
  }
}
</style>
