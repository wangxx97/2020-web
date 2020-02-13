<template>
    <div>
        <!-- 轮播图区域 -->
<!--         <swiper :lunbotuList="lunbotuList" :isfull="true"></swiper>-->
        <div class="swiper-container">
            <div class="swiper-wrapper">
                <div class="swiper-slide">
                    <img class="images" src="../../images/1.png" alt="">
                </div>
                <div class="swiper-slide">
                    <img class="images" src="../../images/2.jpg" alt="">
                </div>
                <div class="swiper-slide">
                    <img class="images" src="../../images/3.png" alt="">
                </div>
            </div>
            <!-- 如果需要分页器 -->
            <div class="swiper-pagination"></div>

            <!-- 如果需要导航按钮 -->
            <div class="swiper-button-prev"></div>
            <div class="swiper-button-next"></div>

            <!-- 如果需要滚动条 -->
            <div class="swiper-scrollbar"></div>
        </div>

        <ul class="mui-table-view mui-grid-view mui-grid-9">
            <li class="mui-table-view-cell mui-media mui-col-xs-4 mui-col-sm-3">
                <router-link to="/home/newslist">
                    <img src="../../images/menu1.png" alt="">
                    <div class="mui-media-body">新闻资讯</div>
                </router-link>
            </li>
            <li class="mui-table-view-cell mui-media mui-col-xs-4 mui-col-sm-3">
                <router-link to="/home/photolist">
                    <img src="../../images/menu2.png" alt="">
                    <div class="mui-media-body">图片分享</div>
                </router-link>
            </li>
            <li class="mui-table-view-cell mui-media mui-col-xs-4 mui-col-sm-3">
                <router-link to="/home/goodslist">
                    <img src="../../images/menu3.png" alt="">
                    <div class="mui-media-body">商品购买</div>
                </router-link>
            </li>
            <li class="mui-table-view-cell mui-media mui-col-xs-4 mui-col-sm-3">
                <a href="#">
                    <img src="../../images/menu4.png" alt="">
                    <div class="mui-media-body">留言反馈</div>
                </a>
            </li>
            <li class="mui-table-view-cell mui-media mui-col-xs-4 mui-col-sm-3">
                <a href="#">
                    <img src="../../images/menu5.png" alt="">
                    <div class="mui-media-body">视频专区</div>
                </a></li>
            <li class="mui-table-view-cell mui-media mui-col-xs-4 mui-col-sm-3">
                <a href="#">
                    <img src="../../images/menu6.png" alt="">
                    <div class="mui-media-body">联系我们</div>
                </a>
            </li>
        </ul>

    </div>
</template>


<script>
    import swiper from "../../swiper.js";
    import {Toast} from "mint-ui";
    // import swiper from "../subcomponents/swiper.vue";
    // export default {
    //     data() {
    //         return {
    //             lunbotuList: [] // 保存轮播图的数组
    //         };
    //     },
    //     created() {
    //         this.getLunbotu();
    //     },
    //     methods: {
    //         getLunbotu() {
    //             // 获取轮播图数据的方法
    //             this.$http.get("api/getlunbo").then(result => {
    //                 // console.log(result.body);
    //                 if (result.body.status === 0) {
    //                     // 成功了
    //                     this.lunbotuList = result.body.message;
    //                 } else {
    //                     // 失败的
    //                     Toast("加载轮播图失败。。。");
    //                 }
    //             });
    //         }
    //     },
    //     components: {
    //         swiper
    //     }
    // };
    var mySwiper = new Swiper('.swiper-container', {
        direction: 'vertical', // 垂直切换选项
        loop: true, // 循环模式选项

        // 如果需要分页器
        pagination: {
            el: '.swiper-pagination',
        },
        // 如果需要前进后退按钮
        navigation: {
            nextEl: '.swiper-button-next',
            prevEl: '.swiper-button-prev',
        },
        // 如果需要滚动条
        // scrollbar: {
        //     el: '.swiper-scrollbar',
        // },
    })


</script>

<style lang="scss" scoped>
    .mui-grid-view.mui-grid-9 {
        background-color: #fff;
        border: none;

        img {
            width: 60px;
            height: 60px;
        }

        .mui-media-body {
            font-size: 13px;
        }
    }

    .mui-grid-view.mui-grid-9 .mui-table-view-cell {
        border: 0;
    }

    .swiper-container {
        width: 100%;
        height: 200px;
    }

    .images {
        width: 100%;
        height: 200px;
    }
</style>
