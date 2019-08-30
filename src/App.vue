<template>
    <div id="app">
        <router-view/>
        <div class="menu">
            <van-row>
                <van-col span="8">
                    <router-link to="/">首页</router-link>
                </van-col>
                <van-col span="8">
                    <router-link to="/list">商品列表</router-link>
                </van-col>
                <van-col span="8">
                    <router-link to="/user">个人中心</router-link>
                </van-col>
            </van-row>
        </div>
    </div>
</template>
<style lang="less">
    body {
        height: 100%;
    }
    .menu {
        position: fixed;
        bottom: 0;
        width: 100%;
        text-align: center;
        box-shadow: 0 -3px 5px -5px #333;
        height: 40px;
        line-height: 40px;
        .van-col {
            font-size: 13px;
            a {
                color: #666;
                display: inline-block;
                width: 100%;
                height: 100%;
            }
        }
        .van-col + .van-col {
            border-left: 1px solid #ddd;
        }
    }
</style>
