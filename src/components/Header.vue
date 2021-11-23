<template>
  <header class="container d-flex align-items-center">
       <div class="logo">
           <img src="@/assets/dc-logo.png" alt="DC logo">
       </div>

       <nav class="flex-grow-1">
           <ul class="d-flex justify-content-end">
               <li>
                   <a href="/">Characters</a>
               </li>
               <li>
                   <a href="/">Comics</a>
               </li>
               <li>
                   <a href="/">Movies</a>
               </li>
               <li>
                   <a href="/">TV</a>
               </li>
               <li>
                   <a href="/">Games</a>
               </li>
               <li>
                   <a href="/">Collectibles</a>
               </li>
               <li>
                   <a href="/">Videos</a>
               </li>
               <li>
                   <a href="/">Fans</a>
               </li>
               <li>
                   <a href="/">News</a>
               </li>
               <li>
                   <a href="/">Shop</a>
               </li>
           </ul>
       </nav>
  </header>
</template>

<script>
export default {
    name: 'Header',

}
</script>

<style scopes lang="scss">
@import '../styles/utilities.scss';

header {
    font-size: 0.65em;
    font-weight: 600;
    .logo {
        margin: 18px auto;
        img {
            max-width: 80px;
        }
    }
    ul {
        list-style: none;
        text-transform: uppercase;
        li {
            margin: 0 17px;
            a {
                text-decoration: none;
            }
        }
    }
}
</style>