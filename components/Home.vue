<template>
    <article>
        <!-- banner begin -->
        <div class="picsbox">
            <slide></slide>
            <top-pic></top-pic>
            <div class="blank"></div>
            <blog></blog>
            <side-bar></side-bar>
        </div>
        <!-- banner end -->
    </article>
</template>
<script>
import Slide from './home/Slide'
import TopPic from './home/TopPic'
import Blog from './home/Blog'
import SideBar from './SideBar'

export default {
    components: {
        Slide,
        TopPic,
        Blog,
        SideBar
    }
}
</script>

