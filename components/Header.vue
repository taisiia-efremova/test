<template>
 <div class="container">
  <div class="links">
    <ul class="main-menu">
      <li>
          <h2>Books</h2>
          <ul class="sub-menu">
            <li><nuxt-link to="/books/classic" class="button--green">Classic</nuxt-link></li>
            <li><nuxt-link to="/books/adventure" class="button--green">Adventure</nuxt-link></li>
          </ul>
      </li>
      <li>
          <h2>Phones</h2>
           <ul class="sub-menu">
            <li><nuxt-link to="/phones/android" class="button--green">Android</nuxt-link></li>
            <li><nuxt-link to="/phones/iphone" class="button--green">Iphone</nuxt-link></li>
          </ul>
      </li>
     </ul>
   </div>
 </div>
</template>

<script>
export default {

}
</script>

<style scoped>
 li {
    list-style:none;
    padding: 10px;
}
</style>