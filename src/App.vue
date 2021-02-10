<template>
  <div class="app">
    <header>
      <h1>The<strong>SciFi</strong>Database</h1>
      <form class="search-box">
        <input
          type="search"
          class="search-field"
          placeholder="Search for SciFi movies..."
          required
        />
      </form>
    </header>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss">
@import url('https://fonts.googleapis.com/css2?family=Nunito+Sans&display=swap');

* {
  box-sizing: border-box;
  padding: 0;
  margin: 0;

  font-family: 'Nunito Sans', sans-serif;
  font-size: 62.5%;
  // border: red 1px solid;
}

a {
  text-decoration: none;
}

header {
  padding-top: 4rem;
  padding-bottom: 4rem;

  h1 {
    color: #888;
    font-size: 5rem;
    font-weight: 400;
    text-align: center;
    text-transform: uppercase;
    margin-bottom: 3rem;

    strong {
      font-size: 5rem;
      color: #313131;
    }

    &:hover {
      color: darken(#313131, 10%);
    }
  }

  .search-box {
    display: flex;
    justify-content: center;
    padding: 0 40px;

    .search-field {
      appearance: none;
      background: none;
      border: none;
      outline: none;

      background-color: #f3f3f3;

      display: block;
      width: 100%;
      max-width: 600px;
      padding: 1.5rem;
      border-radius: 8px;

      color: #313131;
      font-size: 2rem;

      transition: 0.4s;

      &::placeholder {
        color: #aaa;
      }
      &:focus,
      &:valid {
        color: #fff;
        background-color: #313131;
      }
    }
  }
}
</style>
