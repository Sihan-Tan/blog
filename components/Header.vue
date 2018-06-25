<template>
    <header class="menu">
        <el-menu
          :default-active="activeIndex"
          class="nav"
          background-color="#000"
          mode="horizontal"
          @select="handleSelect"
          text-color="#ccc"
          active-text-color="#ffd04b">
          <el-menu-item index="1" style="color: #00a7eb;font-size:16px;margin-right: 50px;">Orialian</el-menu-item>
          <el-menu-item index="2">首页</el-menu-item>
          <el-menu-item index="3">关于我</el-menu-item>
          <el-menu-item index="4">学无止境</el-menu-item>
          <el-menu-item index="5">慢生活</el-menu-item>
        </el-menu>
        <div class="flower">
          <css-doodle>
            :doodle { 
              @grid: 1x10 / 61.8vmin; 
            }

            @place-cell: center; 
            @size: calc(@index() * 10%);
            
            border-radius: 50%;
            border-style: dashed;
            border-width: calc(@index() * 1vmin); 
            border-color: hsla(
              calc(20 * @index()), 70%, 68%, 
              calc(3 / @index() * .8)
            );
            
            --d: @rand(20s, 40s); 
            --rf: @rand(360deg);
            --rt: calc(var(--rf) + @pick(1turn, -1turn));

            animation: spin var(--d) linear infinite;
            @keyframes spin {
              from { transform: rotate(var(--rf)) }
              to   { transform: rotate(var(--rt)) }
            }
          </css-doodle> 
        </div>
    </header>
</template>
<script>
export default {
  name: "Header",
  data() {
      return {
        activeIndex: '2'
      };
    },
    methods: {
      handleSelect(key, keyPath) {
        console.log(key, keyPath);
      }
    }
};
</script>
<style scoped>
.flower {
  width: 50px;
  height: 50px;
  position: relative;
}
</style>
