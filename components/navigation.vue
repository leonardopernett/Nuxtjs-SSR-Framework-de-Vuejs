<template>
    <header>
      <h1>posts app</h1>
      <nav>
          <ul>
              <li>
                  <nuxt-link to="/">Home</nuxt-link>
              </li>
               <li>
                  <nuxt-link to="/posts">posts</nuxt-link>
              </li>
              <li>
                  <nuxt-link to="/about">about</nuxt-link>
              </li>
          </ul>
      </nav>
    </header>
</template>


<script>
export default {
    name:'Navigation'
}
</script>