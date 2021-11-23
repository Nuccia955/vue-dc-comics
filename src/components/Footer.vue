<template>
  <footer>
    <div class="d-flex container justify-content-between">
        <nav class="useful-links d-flex">
            <div class="column">
                <h3>DC Comics</h3>
                <ul>
                    <li>
                        <a href="/">link</a>
                    </li>
                </ul>

                <h3>Shop</h3>
                <ul>
                    <li>
                        <a href="/">link</a>
                    </li>
                </ul>
            </div>

            <div class="column">
                <h3>DC</h3>
                <ul>
                    <li>
                        <a href="">link</a>
                        </li>
                </ul>
            </div>

            <div class="column">
                <h3>Sites</h3>
                <ul>
                    <li>
                        <a href="">link</a>
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
            <a class="d-inline-block" href="/">Sign-Up Now!</a>
            <nav>
                <ul class="d-flex justify-content-end">
                    <li>
                        <a href="/">link</a>
                    </li>
                    <li>
                        <a href="/">link</a>
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
                }
            ul {
                margin-bottom: 30px;
                list-style: none;
                li {
                    padding: 12px 0;
                    a {
                        text-decoration: none;
                        color: #fff;
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
            list-style: none;
            li {
                margin-right: 15px;
                a {
                    color: #fff;
                    text-decoration: none;
                }
            }
        }
    }
    
}

</style>