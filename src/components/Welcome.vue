<script setup>
  import 'animate.css'
  import Button from '../components/Button.vue'
</script>

<template>
  <main class="container">
    <div class="content">
      <div class= "news">
        <b class="animate__animated animate__fadeInUp">Every science news is here!</b>
        <Button class="btn" text="Check it out" title="See the news" />
      </div>
      <img class="cyborg animate__animated animate__fadeInRight" src='../assets/images/cyborg-kv-man.png' alt="" />
    </div>
  </main>
  <img class="background" src="../assets/images/background.jpg" alt="" />
  <span class="filter">
  </span>
</template>

<style lang="scss">

.background {
  position: absolute;
  top: 0;
  left: 0;
  z-index: -1;
  width: 100%;
  height: 30rem;
}

.filter {
  position: absolute;
  top: 10rem;
  left: 0;
  width: 100%;
  height: 20rem;
  background-image: linear-gradient(180deg, rgba(118, 30, 177, 0.336), rgba(122, 255, 255, 0.623));
  z-index: -1;
  filter: blur(1rem);

&::before {
  content: "";
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
}
}

.container {
  height: 100%;
  display: flex;
  align-items: center;
  justify-content: center;
  margin-top: 5rem;

.content {
    display: flex;
    align-items: center;
    justify-content: center;

    .news {
      display: flex;
      align-items: center;
      justify-content: center;
      flex-direction: column;
      background-color: rgba(0, 0, 0, 0.342);
      padding: 2rem 1rem 2rem 1rem;
      border-radius: 20px;
      height: 10rem;
    }
  }
  
  b {
    color: white;
    font-size: 2rem;
    text-align: center;
    text-shadow: 0 0 1rem rgb(0, 0, 0);
}

  .cyborg {
    width: 25%;
    margin-left: 5rem;
  }
}

</style>