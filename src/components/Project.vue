<template>
  <main>
    <div class="main">
      <div class="wrap">
        <span class="ribbon6">项目经历</span>
      </div>
      <h2>项目展示</h2>
      <div class="line"></div>
      <div class="job">
        <h4>Vue 全家桶搭建 CNode 社区</h4>
        <div class="inner">
          <div class="msg">
            <p>该项目调用 CNode 官方社区提供的 API，以 Vue CLI 创建项 目模板，使用 Axios 获取数据，使用 Vue Router 进行前端路由的切换及 传参，使用 watch 监听路由的变化，实现查看帖子，查看用户信息， 不同主题的切换等功能。</p>
            <p>技术栈：Vue.js、Vue-cli、Vuex、ES6、Vue Router、Axios</p>
            <a target="_blank" href="https://github.com/xyyojl/vue-cnode">
              <button class="link">代码链接</button>
            </a>
            <a target="_blank" href="https://xyyojl.github.io/vue-cnode/dist/index.html#/">
              <button class="link">预览链接</button>
            </a>
          </div>
          <img src="../assets/images/pro1.png">
        </div>
      </div>
      <div class="job">
        <h4>Vue 全家桶搭建 CNode 社区</h4>
        <div class="inner">
          <div class="msg">
            <p>该项目调用 CNode 官方社区提供的 API，以 Vue CLI 创建项 目模板，使用 Axios 获取数据，使用 Vue Router 进行前端路由的切换及 传参，使用 watch 监听路由的变化，实现查看帖子，查看用户信息， 不同主题的切换等功能。</p>
            <p>技术栈：Vue.js、Vue-cli、Vuex、ES6、Vue Router、Axios</p>
            <a target="_blank" href="https://github.com/xyyojl/vue-cnode">
              <button class="link">代码链接</button>
            </a>
            <a target="_blank" href="https://xyyojl.github.io/vue-cnode/dist/index.html#/">
              <button class="link">预览链接</button>
            </a>
          </div>
          <img src="../assets/images/pro1.png">
        </div>
      </div>
      <div class="job">
        <h4>Vue 全家桶搭建 CNode 社区</h4>
        <div class="inner">
          <div class="msg">
            <p>该项目调用 CNode 官方社区提供的 API，以 Vue CLI 创建项 目模板，使用 Axios 获取数据，使用 Vue Router 进行前端路由的切换及 传参，使用 watch 监听路由的变化，实现查看帖子，查看用户信息， 不同主题的切换等功能。</p>
            <p>技术栈：Vue.js、Vue-cli、Vuex、ES6、Vue Router、Axios</p>
            <a target="_blank" href="https://github.com/xyyojl/vue-cnode">
              <button class="link">代码链接</button>
            </a>
            <a target="_blank" href="https://xyyojl.github.io/vue-cnode/dist/index.html#/">
              <button class="link">预览链接</button>
            </a>
          </div>
          <img src="../assets/images/pro1.png">
        </div>
      </div>
    </div>
  </main>
</template>

<script>
export default {
  name: 'Project'
}
</script>

<style scoped>
.msg > a {
  color: blue;
  font-weight: bold;
  font-size: 16px;
}
h4 {
  margin-bottom: 0;
}
.main > .line {
  width: 120px;
}
.job {
  padding-bottom: 25px;
  border-bottom: 1px solid #607d8b;
}
.job > .inner {
  display: flex;
}
.msg {
  flex: 1;
}
.inner > img {
  height: 187.5px;
  /* width: 269.8px; */
  margin-left: 10px;
}
.link {
  height: 40px;
  font-size: 16px;
  border-radius: 2px;
  outline: none;
  padding: 0 1em;
  border: none;
  /* background: #607d8b; */
  background: rgb(64, 158, 255);
  color: #f0f0f0;
  cursor: pointer;
}
@media (max-width: 768px) {
  img {
    display: none;
  }
} 
</style>
