<template>
  <el-carousel class="banner" :height="clientHeight" :interval="5000" arrow="hover">
    <el-carousel-item class="slide" v-for="item in imgSrc" :key="item">
      <img :src="item">
    </el-carousel-item>
  </el-carousel>
</template>
<script>
export default {
    data() {
        return {
            imgSrc: [
                'images/banner01.jpg',
                'images/banner02.jpg',
                'images/banner03.jpg',
            ],
            clientHeight: '360px'
        }
    },
    methods: {
        getSlideHeight() {
            let width = `${document.documentElement.clientWidth}`
            if(width >= 1200) {
                this.clientHeight = '450px'
            }else if(width >= 1024) {
                this.clientHeight = '360px'
            }else if(width >= 960) {
                this.clientHeight = '337px'
            }else if(width >= 768) {
                this.clientHeight = '279px'
            }
            return this.clientHeight
        }
    },
    mounted() {
        this.getSlideHeight()
    }
}
</script>

