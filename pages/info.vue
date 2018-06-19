<template>
    <div>
        <div class="pagebg sh"></div>
        <div class="container">
            <h1 class="t_nav">
                <span>不要轻易放弃。学习成长的路上，我们长路漫漫，只因学无止境。 </span>
                <a href="/" class="n1">网站首页</a><a href="/" class="n2">慢生活</a></h1>
            <info></info>
            <side-bar></side-bar>
        </div>
    </div>
</template>
<script>
import Info from '~/components/Info'
import SideBar from '~/components/SideBar'
export default {
    components: {
        Info,
        SideBar
    }
}
</script>

