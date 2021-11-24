<template>
  <header class="container d-flex align-items-center">
       <div class="logo">
           <img src="@/assets/dc-logo.png" alt="DC logo">
       </div>

       <nav class="flex-grow-1">
           <ul class="d-flex justify-content-end">
               <li v-for="(link, index) in links" :key="`link-${index}`">
                   <a  class="d-inline-block" :href="link.href">{{ link.text }}</a>
               </li>
           </ul>
       </nav>
  </header>
</template>

<script>
export default {
    name: 'Header',
    data() {
        return {
            links: [
                {
                    text: 'Characters',
                    href: '/',
                    active: false,        
                },
                {
                    text: 'Comics',
                    href: '/',
                    active: false,        
                },
                {
                    text: 'Movies',
                    href: '/',
                    active: false,         
                },
                {
                    text: 'TV',
                    href: '/',
                    active: false,         
                },
                {
                    text: 'Games',
                    href: '/',
                    active: false,         
                },
                {
                    text: 'Collectibles',
                    href: '/',
                    active: false,         
                },
                {
                    text: 'Videos',
                    href: '/',
                    active: false,         
                },
                {
                    text: 'Fans',
                    href: '/',
                    active: false,         
                },
                {
                    text: 'News',
                    href: '/',
                    active: false,         
                },
                {
                    text: 'Shop',
                    href: '/',
                    active: false,         
                },
            ],
        }   
    }

}
</script>

<style scopes lang="scss">
@import '../styles/utilities.scss';

header {
    font-size: 0.7em;
    font-weight: 600;
    .logo {
        margin: 18px auto;
        img {
            max-width: 80px;
        }
    }
    ul {
        text-transform: uppercase;
        li {
            margin: 0 17px;
            a {
                color: #464657;

                &:hover,
                &:active {
                    color: #0282f9;
                }
            }
        }
    }
}
</style>