<template>
  <footer>
    <div class="d-flex container justify-content-between">
        <nav class="useful-links d-flex">
            <div class="column">
                <h3>DC Comics</h3>
                <ul>
                    <li v-for="(link, index) in dcComicsLinks" :key="`comics-link ${index}`">
                        <a :href="link.href">{{ link.text }}</a>
                    </li>
                </ul>

                <h3>Shop</h3>
                <ul>
                    <li v-for="(link, index) in shopLinks" :key="`shop-link ${index}`">
                        <a :href="link.href">{{ link.text }}</a>
                    </li>
                </ul>
            </div>

            <div class="column">
                <h3>DC</h3>
                <ul>
                    <li v-for="(link, index) in dcLinks" :key="`dc-link ${index}`">
                        <a :href="link.href">{{ link.text }}</a>
                    </li>
                </ul>
            </div>

            <div class="column">
                <h3>Sites</h3>
                <ul>
                    <li v-for="(link, index) in sites" :key="`sites-link ${index}`">
                        <a :href="link.href">{{ link.text }}</a>
                    </li>
                </ul>
            </div>
        </nav>

        <div class="logo">
            <img src="@/assets/dc-logo-bg.png" alt="DC logo">
        </div>
    </div>

    <div class="position-fixed">
        <div class="container d-flex justify-content-between align-items-center">
            <a class="d-inline-block btn" href="/">Sign-Up Now!</a>
            <nav class="d-flex">
                <ul class="d-flex justify-content-end align-items-center">
                    <li>
                        <a  class="follow-us" href="/">Follow Us</a>
                    </li>
                    <li>
                        <a href="/">
                            <img src="../assets/footer-facebook.png" alt="facebook">
                        </a>
                    </li>
                    <li>
                        <a href="/">
                            <img src="../assets/footer-twitter.png" alt="facebook">
                        </a>
                    </li>
                    <li>
                        <a href="/">
                            <img src="../assets/footer-youtube.png" alt="facebook">
                        </a>
                    </li>
                    <li>
                        <a href="/">
                            <img src="../assets/footer-pinterest.png" alt="facebook">
                        </a>
                    </li>
                    <li>
                        <a href="/">
                            <img src="../assets/footer-periscope.png" alt="facebook">
                        </a>
                    </li>
                </ul>
            </nav>
        </div>
    </div>
  </footer>
</template>

<script>
export default {
    name: 'Footer',
    data() {
        return {
            dcComicsLinks: [
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
                    text: 'Videos',
                    href: '/',
                    active: false,         
                },
                {
                    text: 'News',
                    href: '/',
                    active: false,         
                },
            ],
            shopLinks: [
                {
                    text: 'Shop DC',
                    href: '/',
                    active: false,   
                },
                {
                    text: 'Shop DC Collectibles',
                    href: '/',
                    active: false,   
                }
            ],
            dcLinks: [
                {
                    text: 'Terms Of Use',
                    href: '/',
                    active: false,   
                },
                {
                    text: 'Privacy Policy (New)',
                    href: '/',
                    active: false,   
                },
                {
                    text: 'Ad Choices',
                    href: '/',
                    active: false,   
                },
                {
                    text: 'Advertising',
                    href: '/',
                    active: false,   
                },
                {
                    text: 'Job',
                    href: '/',
                    active: false,   
                },
                {
                    text: 'Subscriptions',
                    href: '/',
                    active: false,   
                },
                {
                    text: 'Talent Workshops',
                    href: '/',
                    active: false,   
                },
                {
                    text: 'CPSC Certificates',
                    href: '/',
                    active: false,   
                },
                {
                    text: 'Ratings',
                    href: '/',
                    active: false,   
                },
                {
                    text: 'Shop Help',
                    href: '/',
                    active: false,   
                },
                {
                    text: 'Contact Us',
                    href: '/',
                    active: false,   
                },
            ],
            sites: [
                {
                    text: 'DC',
                    href: '/',
                    active: false,   
                },
                {
                    text: 'MAD Magazines',
                    href: '/',
                    active: false,   
                },
                {
                    text: 'DC Kids',
                    href: '/',
                    active: false,   
                },
                {
                    text: 'DC Universe',
                    href: '/',
                    active: false,   
                },
                {
                    text: 'DC Power Visa',
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

footer {
    background-image: url('../assets/footer-bg.jpg');
    nav.useful-links {
        padding: 40px 0 60px 0;
    }
    nav {
        .column {
            margin-right: 55px;
            h3 {
                    text-transform: uppercase;
                    color: #fff;
                    margin-bottom: 12px;
                }
            ul {
                margin-bottom: 30px;
                li {
                    padding: 5px 0;
                    font-size: 0.75em;
                    a {
                        color: #959595;
                        &:hover,
                        &:active {
                            text-decoration: underline;
                        }
                    }
                }
            }
        }
    }
    & > div:last-child {
        width: 100%;
        bottom: 0;
        background-color: #303030;
        padding: 30px 0;

        & > div >  a {
            color: #fff;
            text-decoration: none;
            border: 3px solid #0282f9;
            text-transform: uppercase;
            padding: 17px;
        }
        ul {
            li {
                margin-right: 15px;
                a.follow-us {
                            color: #0282f9;
                            text-transform: uppercase;
                            font-weight: 600;
                            margin-right: 15px;
                        }
            }
        }
    }
    
}

</style>