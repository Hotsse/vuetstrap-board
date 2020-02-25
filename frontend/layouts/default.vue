<template>
  <div>
    <div class="jumbotron text-center" style="margin-bottom:0">
      <h1>My First Bootstrap 4 Page</h1>
      <p>Resize this responsive page to see the effect!</p>
    </div>

    <nav class="navbar navbar-expand-sm bg-dark navbar-dark">
      <nuxt-link to="/" class="navbar-brand">Home</nuxt-link>
      <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#collapsibleNavbar">
        <span class="navbar-toggler-icon" />
      </button>
      <div id="collapsibleNavbar" class="collapse navbar-collapse">
        <ul class="navbar-nav">
          <li class="nav-item">
            <nuxt-link to="/about" class="nav-link">About</nuxt-link>
          </li>
          <li class="nav-item">
            <nuxt-link to="/board/list" class="nav-link">Board</nuxt-link>
          </li>
        </ul>
      </div>
    </nav>

    <nuxt />

    <div class="jumbotron text-center" style="margin-bottom:0">
      <p>Footer</p>
    </div>
  </div>
</template>

<script>
export default {
  scrollToTop: false
}
</script>

<style>
html {
  font-family: 'Source Sans Pro', -apple-system, BlinkMacSystemFont, 'Segoe UI',
    Roboto, 'Helvetica Neue', Arial, sans-serif;
  font-size: 16px;
  word-spacing: 1px;
  -ms-text-size-adjust: 100%;
  -webkit-text-size-adjust: 100%;
  -moz-osx-font-smoothing: grayscale;
  -webkit-font-smoothing: antialiased;
  box-sizing: border-box;
}

*,
*:before,
*:after {
  box-sizing: border-box;
  margin: 0;
}

.button--green {
  display: inline-block;
  border-radius: 4px;
  border: 1px solid #3b8070;
  color: #3b8070;
  text-decoration: none;
  padding: 10px 30px;
}

.button--green:hover {
  color: #fff;
  background-color: #3b8070;
}

.button--grey {
  display: inline-block;
  border-radius: 4px;
  border: 1px solid #35495e;
  color: #35495e;
  text-decoration: none;
  padding: 10px 30px;
  margin-left: 15px;
}

.button--grey:hover {
  color: #fff;
  background-color: #35495e;
}
</style>
