<template>
<nav class="tabs">
    <li class="tab">
        <router-link to='/home'>
            <i class="iconfont icon-home"></i>
            <span>首页</span>
        </router-link>
    </li>
    <li class="tab">
        <router-link to='/category'>
            <i class="iconfont icon-category"></i>
            <span>分类</span>
        </router-link>
    </li>
    <li class="tab">
        <router-link to='/cart'>
            <i class="iconfont icon-cart"></i>
            <span>购物车</span>
        </router-link>
    </li>
    <li class="tab">
        <router-link to='/mine'>
            <i class="iconfont icon-mine"></i>
            <span>我的</span>
        </router-link>
    </li>
</nav>
</template>

<script>
export default {
    name: 'app-tabs'
}
</script>
<style lang="scss" scoped>
.tabs{
    width:100%;
    height: 49px;
    position: absolute;
    left: 0;
    bottom: 0;
    background: #ffffff;
    display: flex;
    .tab{
        flex: 1;
        a{
            display: block;
            width: 100%;
            height: 100%;
            display: flex;
            flex-direction: column;
            i{
                display: block;
                font-size: 18px;
                margin: 0 auto;
                color:#999;
                margin-top: 6px;
            }
            &.router-link-active i{
                color: #ff6700;
            }
            span{
                display: block;
                font-size: 12px;
                color: #999;
                text-align: center;
                margin-top: 3px;
            }
            &.router-link-active span{
                color: #ff6700;
            }
        }
    }
}
</style>

