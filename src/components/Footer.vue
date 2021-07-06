<template>
    <footer>
        <div class="container footer">
            <div class="all-links-container">
                <div class="column">
                    <ul>
                        <li>DC Comics</li>
                        <li><a href="#">Characters</a></li>
                        <li><a href="#">Comics</a></li>
                        <li><a href="#">Movies</a></li>
                        <li><a href="#">TV</a></li>
                        <li><a href="#">Games</a></li>
                        <li><a href="#">Videos</a></li>
                        <li><a href="#">News</a></li>
                    </ul>
                    <ul>
                        <li>DC Shop</li>
                        <li><a href="#">Shop DC</a></li>
                        <li><a href="#">Shop DC Collectibles</a></li>
                    </ul>
                </div>

                <div class="column">
                    <ul>
                        <li>DC</li>
                        <li><a href="#">Terms of Use</a></li>
                        <li><a href="#">Privacy Policy (New)</a></li>
                        <li><a href="#">Ad Choices</a></li>
                        <li><a href="#">Advertising</a></li>
                        <li><a href="#">Jobs</a></li>
                        <li><a href="#">Subscriptions</a></li>
                        <li><a href="#">CPSC Certificates</a></li>
                        <li><a href="#">Ratings</a></li>
                        <li><a href="#">Shop Help</a></li>
                        <li><a href="#">Contact Us</a></li>
                    </ul>
                </div>

                <div class="column">
                    <ul>
                        <li>Sites</li>
                        <li><a href="#">DC</a></li>
                        <li><a href="#">DC UNIVERSE INFINITE</a></li>
                        <li><a href="#">DC Kids</a></li>
                        <li><a href="#">DC Shop</a></li>
                        <li><a href="#">MAD Magazine</a></li>
                    </ul>
                </div>
                    
            </div>
            <!-- <div class="logo-img">
                <img src="../assets/img/dc-logo-bg.png" alt="">
            </div> -->

        </div>
        
    </footer>
  
</template>

<script>
export default {
    name:'Footer'

}
</script>

<style lang='scss'>
@import '@/style/vars.scss';

footer{
    background-image: url('../assets/img/footer-bg.jpg');
    background-size: cover;
    
    .footer{
        background-image: url('../assets/img/dc-logo-bg.png');
        background-size: 450px;
        background-repeat: no-repeat;
        background-position: right center;
        padding: 20px 0 50px 0;
        display: flex;
        justify-content: flex-start;


        .all-links-container{
            display: flex;

            .column{
                margin-right:20px;

                li{
                    list-style: none;
                    color: white;
                    font-size:$fsize-md;
                    font-weight: $weight-font;
                    
                    &:first-child{
                        text-transform: uppercase;
                        margin: 15px 0 8px 0;
                    }

                    a{
                    text-decoration:none;
                    color:$light;
                    font-size: 12px;
                }
                }

                
            }


        }
        
    }
}

</style>