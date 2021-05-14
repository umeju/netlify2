<template>

<div>

  <a :href="url" :class="classess" :dir="testo"> {{indirizzo | uppercase}}  - [vedi questo]     </a>

  <p @click="clicked" :class="classess"> PULSANTE  </p>

  <slot></slot>
  <p>     this is the new comp --> {{testo}}    </p>


</div>
 
</template>


<script>
export default {
  
  methods: {
    clicked() {
      this.cl = !this.cl
    },
    capitalize() {
      return 
    }
  },

  props: [
    'dir'
  ],
  computed: {
    classess() {
      return this.cl ? 'rosso' : 'verde'
    }
  },

  data() {
    return {
      indirizzo: "fb://facewebmodal/f?href=https://www.facebook.com/www.hubanero.it",
      testo: 'testo scritto',
      cl: false,
      url: "#"
    }
  },
  filters: {
        uppercase: function(value) {
            return value.toUpperCase() || "";
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
.rosso {
  color: red;
}
.verde {
  color: green;
}

</style>
