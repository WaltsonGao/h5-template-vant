<template>
    <div class="user-center">
        <van-row class="user-info">
            <van-image
                width="100"
                height="100"
                src="https://img.yzcdn.cn/vant/cat.jpeg"
            />
            <div>
                Big Cat
            </div>
        </van-row>
        <van-cell-group>
            <van-cell title="积分" value="2200" />
            <van-cell title="联系方式" value="18810667062" />
            <van-cell title="入驻日期" value="2018-12-12" />
            <van-cell title="地址" value="浙江省杭州市滨江区长河路331号" />
        </van-cell-group>
    </div>
</template>
<script>
export default {
    data() {
        return {
            userName: '',
            userAvatar: '',
        };
    },
    methods: {
        onClickLeft() {
            this.$router.push('/');
        },
    }
};
</script>
<style lang="less">
    .user-center {
        .user-info {
            padding: 40px 0 20px;
            .van-image {
                margin: 0 auto;
                display: block;
                padding-bottom: 10px;
                img {
                    border-radius: 10px;
                }
            }
            text-align: center;
        }
    }
</style>
