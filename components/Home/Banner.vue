 <!-- 首页 海报轮播图组件 -->
<template>
    <section class="banner">
        <div class="banner_outside">
            <div class="banner_inside">
                <div class="bannerurl"> 
                    <a href="">了解详情</a>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
@import '../../assets/style.scss';

.banner {
    width: 100%;
    background: url('../../static/images/home/banner_background.png');
    z-index: 1;
    position: absolute;
    top: 0;
    left: 0;
    .banner_outside {
        
        .banner_inside {
            height: vm(622);
            width: vm(1200);
            margin: 0 auto;
            position: relative;
            .bannerurl {
                width: vm(190);
                height: vm(35);
                margin: vm(328) auto 0 auto;
                background: url('../../static/images/home/banner_01.png');
                background-size: cover;
                a {
                    background: linear-gradient(105deg, #4dc4d0, #3497dc);
                    display: block;
                    text-align: center;
                    line-height: vm(35);
                    -webkit-background-clip: text;
                    color: transparent;
                    font-size: vm(18);
                    &:hover {
                        color: #fff;
                    }
                }
            }
        }
    }
}
</style>
