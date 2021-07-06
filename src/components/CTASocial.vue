<template>
    <section>
        <div class="container bottom-footer">
            <div class="CTA">
                <h4>sign-up now!</h4>

            </div>
            <div class="social-icons">
                <h3>follow us</h3>
                <img src="../assets/img/footer-facebook.png" alt="facebook icon">
                <img src="../assets/img/footer-twitter.png" alt="Twitter icon">
                <img src="../assets/img/footer-youtube.png" alt="YouTube icon">
                <img src="../assets/img/footer-pinterest.png" alt="Pinterest icon">
                <img src="../assets/img/footer-periscope.png" alt="Periscope icon">
            </div>
        </div>

    </section>
  
</template>

<script>
export default {
    name:'CTASocial'

}
</script>

<style lang='scss' scoped>
@import '@/style/vars.scss';

section{
    background-color: $dark;

    .bottom-footer{
        display: flex;
        align-items: center;
        justify-content: space-between;
        padding: 28px 0;

        .CTA{
            border:2px solid $primary;

            h4{
                color: white;
                text-transform: uppercase;
                padding: 8px 12px;
            }
        }

        .social-icons{
            width: 30%;
            display: flex;
            align-items: center;
            justify-content: space-between;

            h3{
                color: $primary;
                text-transform: uppercase;
            }

            img{
                width:30px
            }
        }
    }
}

</style>