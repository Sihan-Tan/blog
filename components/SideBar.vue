<template>
    <div class="sidebar">
        <zhuan-ti></zhuan-ti>
        <wen-zhang></wen-zhang>
        <pai-hang></pai-hang>
        <biao-qian></biao-qian>
        <lian-jie></lian-jie>
        <guan-zhu></guan-zhu>
    </div>
</template>

<script>
import ZhuanTi from './sidebar/ZhuanTi'
import WenZhang from './sidebar/WenZhang'
import PaiHang from './sidebar/PaiHang'
import BiaoQian from './sidebar/BiaoQian'
import LianJie from './sidebar/Lianjie'
import GuanZhu from './sidebar/GuanZhu'

export default {
    components: {
        ZhuanTi,
        WenZhang,
        PaiHang,
        BiaoQian,
        LianJie,
        GuanZhu
    }
}
</script>

