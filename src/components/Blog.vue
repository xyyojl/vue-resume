<template>
  <main>
    <div class="main">
      <div class="wrap">
        <span class="ribbon6">我的博客</span>
      </div>
      <h2>博客</h2>
      <div class="line"></div>
      <p>在学习前端技术的历程中，我会将学习后的笔记以及遇到的难点整理为博客，通过这样来记录自己学习的点点滴滴。</p>
      <p>这是我的博客地址：<a target="_blank"  href="https://www.jianshu.com/u/71a9fc012556">xyyojl 的简书博客</a> 。</p>
      <p>我是直接在简书这个平台上写博客，有时我也会把一些博客搬运到 <a target="_blank"  href="https://juejin.im/user/5a25fb0df265da43346fc2c7/posts">掘金</a> 上和大家分享。</p>
      <p>对我而言，写博客不仅仅是对知识的总结和梳理，更重要的是可以跟不同的人交流和探讨问题。</p>
    </div>
  </main>
</template>

<script>
export default {
  name: 'Blog'
}
</script>

<style scoped>
a {
  color: blue;
  text-decoration: underline;
  font-weight: bold;
  user-select: auto;
}
.main > .line {
  width: 60px;
}
</style>
