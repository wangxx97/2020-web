<template>
    <div class="all">
        <!--        <h3>MemberContainer</h3>-->
        <div class="photo">
            <img src="../../images/photo.jpg" alt="">
            <h6 style="color: gold">username:wangxixin</h6>
        </div>

        <div class="use">
            <p>
                <a class="p1">会员分 ></a>
            </p>
            <p>
                <a class="p2">全部订单 ></a>
            </p>
            <p>
                <a class="p3">收藏 ></a>
            </p>
            <p>
                <a class="p4">售后 ></a>
            </p>
        </div>

        <div class="bottom">
            <h6>https://github.com/wangxxx97</h6>
        </div>

    </div>
</template>

<script>
</script>

<style lang="scss" scoped>
    .all {
        width: 100%;
        height: 100%;
        text-align: center;
        /*position: relative;*/
    }

    h3 {
        color: gray;
    }

    img {
        width: 100px;
        height: 100px;
        border-radius: 50%;
    }

    .use {
        margin-top: 20px;
        width: 100%;
        text-align: left;
    }

    a {
        /*transition: none;*/
        color: gray;
    }

    p {
        width: 100%;
        /*border: 1px solid red;*/
        border: 1px solid gainsboro;
    }

    .p1,
    .p2,
    .p3,
    .p4 {
        /*border: 1px solid gainsboro;*/
        padding-left: 20px;
        height: 40px;
        line-height: 40px;
    }

    .p1:hover,
    .p2:hover,
    .p3:hover,
    .p4:hover {
        color: pink;
        cursor: pointer;
    }

    .p1 {
        margin-top: 8px;
    }

    .bottom {
        /*position: absolute;*/
        /*bottom: 0;*/
        margin-top: 20px;
    }


</style>
