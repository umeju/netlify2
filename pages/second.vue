<template>
  <div class="container">
    <div>
      <h1 class="title">printhub</h1>
      <h2>Digital Signage & Software</h2>
      <h3>richiedi le tue nuove qr card</h3>
      <h3>basta un tap!</h3>
      <p class="icons">
        <Tel />
        <Logo />
        <Fb />
        <Ig />
        <Web />
        <Mail />
        <Newcomp />
        <Newcomp>
          <h2>slot</h2>
        </Newcomp>

      </p>
      <div class="links">
        <a
          href="https://www.hubanero.it"
          target="_blank"
          rel="noopener noreferrer"
          class="button--green"
        >
          www.hubanero.it
        </a>
      </div>
    </div>
  </div>
</template>

<script>
import newcomp from '../components/Newcomp.vue'
export default {
  components: { newcomp },

}
</script>
<style>
html {
  background: radial-gradient(
    circle,
    rgba(174, 232, 238, 0.3) 0%,
    rgba(144, 96, 220, 0.6) 100%
  );
  margin: 0 auto;
}
.container {
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}

.title {
  font-family: 'Ubuntu', sans-serif;display: block;
  font-weight: 400;
  font-size: 40px;
  color: white;
  letter-spacing: 1px;
  margin: 23px 0 0 0;
  background-color: #dd4814;
}

.subtitle {
  font-weight: 300;
  font-size: 42px;
  color: #526488;
  word-spacing: 5px;
  padding-bottom: 5px;
}

.links {
  padding-top: 15px;
}
.loghi {
  flex-grow: 1;
  -webkit-animation: appear 1s;
  animation: appear 1s;
  width: 38%;
  height: 160px;
  background-repeat: no-repeat;
  background-position: 50%;
  background-size: 120px;
  display: inline-block;
  padding: 30px;
}
h1 {
  font-family: Verdana, Geneva, sans-serif;
  font-size: 40px;
  letter-spacing: -0.8px;
  color: #137d6a;
  font-weight: 400;
  text-decoration: none;
  font-style: normal;
}
h2 {
  color: #dd4814;
}
.icons {
  margin: 36px 0;
}
.button--green{
  color: white;
  border: 1px solid white;
}
</style>
