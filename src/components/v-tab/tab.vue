<template>
    <div class="v-tab">
        <router-link tag="div" class="tab-item" to="/recommend">
            <span class="tab-link">推荐</span>
        </router-link>
        <router-link tag="div" class="tab-item" to="/singer">
            <span class="tab-link">歌手</span>
        </router-link>
        <router-link tag="div" class="tab-item" to="/rank">
            <span class="tab-link">排行
            </span>
        </router-link>
        <router-link tag="div" class="tab-item" to="/search">
            <span class="tab-link">搜索</span>
        </router-link>
    </div>
</template>

<script>
export default {

}
</script>

<style scoped lang="stylus" rel="stylesheet/stylus">
  @import "~common/stylus/variable"
    .v-tab
        display: flex
        height: 50px
        line-height: 50px
        font-size: $font-size-medium
        background: $color-theme
        .tab-item
            flex: 1
            text-align: center
            .tab-link
                padding-bottom: 5px
                color: $color-text-wl
            &.router-link-active
                .tab-link
                    color: $color-text-w
                    border-bottom: 2px solid $color-text-w
</style>