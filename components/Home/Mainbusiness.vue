<!-- 首页 主营业务 组件 尚未开发完成 -->
<template>
    <section class="mainness">
        <div class="mness_outside">
            <div class="mness_inside">
                <ul class="mness_">
                    <li v-for="mness in mnesslist">
                        <div class="mness_imgText">
                            <img src="../../static/images/home/yewu/yewu_01.png" alt="">
                            <p> {{mness.title}} </p>
                        </div>
                        <p class="mness_content">{{mness.content}}</p>
                        <div class="mness_hover">
                            <h2>关键词</h2>
                            <ul>
                                <li>区块链+</li>
                                <li>区块链+</li>
                                <li>区块链+</li>
                            </ul>
                        </div>
                    </li>
                </ul>
            </div>
        </div>
    </section>
</template>

<script>
export default {
    data() {
        return {
            mnesslist: [
                {
                    img: '../../static/images/home/yewu/yewu_01.png',
                    title: '技术开发',
                    content: '专业开发团队，在区块链+领域拥有丰富经验，根据企业需求定制开发官网、APP、小程序、微商城等平台，同时提供用户自传播的营销工具。'
                },
                {
                    img: '../../static/images/home/yewu/yewu_02.png',
                    title: '项目运维',
                    content: '团队具有广泛的行业经验以及广阔的产业、渠道资源。运维实操过程结合各行业发展趋势和业务特点，进行精准化市场营销、运营，实现项目成功增值。'
                },
                {
                    img: '../../static/images/home/yewu/yewu_03.png',
                    title: '创业投资',
                    content: '轻起来集团拥有雄厚的资金实力与管理经验。依据敏锐的商业眼光，发掘有潜力的合作项目并乐于对其进行资金、管理等方面的扶持，达成合作共赢。'
                }
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
@import '../../assets/style.scss';

.mainness {
    width: 100%;
    height: vm(350);
    position: absolute;
    top: vm(517);
    z-index: 2;
    .mness_outside {
        .mness_inside {
            width: vm(1200);
            margin: 0 auto;
            background: #fff;
            ul {
                display: flex;
                justify-content: space-between;
                li {
                    width: vm(308);
                    padding: 0 vm(30) 0 vm(35);
                    position: relative;
                    .mness_imgText {
                        margin: vm(53) auto vm(24) auto;
                        img {
                            width: vm(67);
                            margin: 0 auto;
                        }
                        p {
                            font-size: vm(24);
                            color: #3eaad7;
                            text-align: center;
                        }
                    }
                    .mness_content {
                        font-size: vm(16);
                        padding-bottom: vm(75);
                    }
                    .mness_hover {
                        width: 100%;
                        height: 100%;
                        position: absolute;
                        top: 0;
                        left: 0;
                        background: url("../../static/images/home/yewu/yewu_backg.png");
                        background-position: top center;
                        h2 {
                            position: absolute;
                            top: vm(98);
                            left: vm(155);
                            color: #fff;
                            font-size: vm(22);
                        }
                        ul li {
                            float: none;
                            background: url("../../static/images/home/yewu/yewu_k.png");
                            background-size: cover;
                        }
                    }
                }
            }
        }
    }
}
</style>

