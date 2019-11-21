<template>
  <main>
    <div class="main">
      <div class="message">
        <h1>我是区家乐</h1>
        <div class="line"></div>
        <p>在我看来，前端工程师能够通过写代码之后，可以直接看到自己做的作品，很有成就感，而且能够接触到很多使用不同技术的小伙伴。</p>
        <p><span class="bold">教育背景</span> 2020 应届本科 五邑大学 信息管理与信息系统</p>
        <p><span class="bold">意向职位</span> 前端开发</p>
        <p>本人思维严谨，有较强的学习及适应能力，热衷探索新鲜技术，常浏览技术网站，关注技术动态。工作主动认真，责任心、执行力及抗压性强。 </p>
        <div class="buttonWrapper">
          <a href="../../static/resume.pdf" download="2019-区家乐-应聘前端开发工程师.pdf">
            <button class="download">下载 PDF 版简历</button>
          </a>
          <router-link :to="{name:'Contact'}">
            <button class="skip">联系我</button>
          </router-link>
        </div>
        <div class="wrap">
          <span class="ribbon6">个人信息</span>
        </div>
      </div>
    </div>
  </main>
</template>

<script>
export default {
  name: 'Message'
}
</script>

<style scoped>
main {
  display: flex;
  flex-direction: column;
}
.main {
  font-size: 18px;
  position: relative;
  background: #fafafa;
  box-shadow: rgba(0, 0, 0, 0.19) 0px 10px 30px,
    rgba(0, 0, 0, 0.23) 0px 6px 10px;
  font-family: 幼圆;
  display: flex;
}
.main > .message {
  flex: 1;
  margin-right: 35px;
}
.message > .line {
  width: 150px;
  border: 1px solid #607d8b;
}
.message > p {
  color: #252728;
  font-size: 16px;
  line-height: 1.6em;
  letter-spacing: 1px;
  font-weight: 300;
}
.message > .buttonWrapper {
  user-select: none;
}
.message > .buttonWrapper button {
  height: 40px;
  font-size: 14px;
  border-radius: 2px;
  outline: none;
  font-weight: bold;
  padding: 0 1em;
  cursor: pointer;
  background: rgb(64, 158, 255);
  color: #fff;
  transition: 0.3s;
  border: none;
}
button.download:hover,
button.skip:hover {
  opacity: 0.8;
}
span.bold {
  font-weight: bold;
}
.wrap {
  position: absolute;
  top: -8px;
  left: -8px;
  overflow: hidden;
  width: 150px;
  height: 150px;
  user-select: none;
}
.wrap::before {
  content: "";
  display: block;
  border-radius: 8px 8px 0px 0px;
  width: 40px;
  height: 8px;
  position: absolute;
  left: 100px;
  background: #212121;
}
.wrap::after {
  content: "";
  display: block;
  border-radius: 0px 8px 8px 0px;
  width: 8px;
  height: 40px;
  position: absolute;
  left: 0px;
  top: 100px;
  background: #212121;
}
.ribbon6 {
  color: #fafafa;
  display: inline-block;
  text-align: center;
  width: 200px;
  height: 40px;
  line-height: 40px;
  position: absolute;
  top: 30px;
  left: -50px;
  z-index: 2;
  overflow: hidden;
  transform: rotate(-45deg);
  border: 1px dashed;
  box-shadow: 0 0 0 3px #607d8b, 0px 21px 5px -18px rgba(0, 0, 0, 0.6);
  background: #607d8b;
}
@media (min-width: 1125px) {
  .main {
    position: fixed;
    margin: 60px 0;
    left: 375px;
    width: calc(100vw - 550px);
    min-height: 400px;
    padding: 50px;
  }
}
@media (max-width: 1125px) {
  .main {
    margin: 40px;
    width: calc(100vw - 180px);
    min-height: 400px;
    padding: 50px;
  }
}
@media (max-width: 550px) {
  .wrap {
    display: none;
  }
  .main {
    width: auto;
    padding: 1em 2em;
    margin: 0;
    min-height: 85vh;
  }
}
@media (max-width: 1200px) and (min-width: 1126px) {
  .main > .message > .buttonWrapper {
    position: absolute;
    top: 450px;
    right: 80px;
  }
}
</style>
