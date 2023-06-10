<template>
  <nav>
    <div class="nav-container">
      <div>
        <b>Future</b>
      </div>
      <div class="paths">
        <p>Home</p>
        <p>About</p>
        <p>Contact</p>
      </div>
    </div>
  </nav>
</template>

<style lang="scss">
nav {
  display: flex;
  justify-content: space-around;
.nav-container {
  display: flex;
  align-items: center;
  justify-content: space-between;
  background-color: rgb(21, 19, 22);
  box-shadow: 0 .3rem 1rem rgba(0, 0, 0, 0.658);
  width: 100vw;
  position: fixed;
  top: 0;
  left: 0;
  z-index: 2;

  b {
    color: white;
    text-transform: uppercase;
    letter-spacing: .2rem;
    font-size: 1.5rem;
    margin-left: 1rem;
    transition: .2s;
    cursor: pointer;

    &:hover {
      color: rgb(199, 199, 199);
    }
  }

  .paths {
    display: flex;
    gap: 1rem;
    margin-right: 1rem;

    p {
      color: white;
      transition: .2s;
      cursor: pointer;
      
      &:hover {
        color: rgb(199, 199, 199);
      }
    }
  }
}
}
</style>