<template>
  <div class="card">
    <a href="#" target="_blank">
      <img src="https://placehold.it/300x500" alt="movie poster" />
      <h3>Alien</h3>
    </a>
  </div>
</template>

<style lang="scss" scoped>
.card {
  flex: 1 1 33%;
  width: 33%;
  max-width: 33%;
  padding: 0px 8px;
  margin-bottom: 16px;

  img {
    width: 100%;
    height: 100%;
    object-fit: cover;
    border-radius: 16px;
    box-shadow: 0px 4px 8px rgba(0, 0, 0, 0.15);
    transition: 0.4s ease-in-out;
  }

  h3 {
    padding: 16px;
    font-size: 3.5rem;
    color: #313131;

    transition: 0.4s ease-in-out;
  }

  &:hover {
    img {
      transform: scale(1.05);
    }

    h3 {
      color: rgb(61, 55, 100);
    }
  }
}
</style>
