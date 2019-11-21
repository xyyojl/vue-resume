<template>
  <aside>
    <img src="../assets/avator.jpg" alt="我的头像">
    <span class="name">区家乐</span>
    <span class="big">区家乐 - 2019 - 应聘前端工程师</span>
    <span class="small">区家乐 xyyojl</span>
    <span class="motto">让优秀成为一种习惯！</span>
    <div class="link">
      <div class="inside">
        <router-link :to="{name:'Message'}">个人</router-link>
      </div>
      <div class="inside">
        <router-link :to="{name:'Skill'}">技能</router-link>
      </div>
      <div class="inside">
        <router-link :to="{name:'Project'}">项目</router-link>
      </div>
      <div class="inside">
        <router-link :to="{name:'Blog'}">博客</router-link>
      </div>
      <div class="inside">
        <router-link :to="{name:'Contact'}">联系我</router-link>
      </div>
    </div>
    <footer class="icons">
      <a href="https://github.com/xyyojl" target="_blank">
        <svg class="icon" aria-hidden="true">
          <use xlink:href="#icon-GitHub"></use>
        </svg>
      </a>
      <a href="#"  target="_blank">
        <svg class="icon" aria-hidden="true">
          <use xlink:href="#icon-zhihu-circle-fill"></use>
        </svg>
      </a>
    </footer>
  </aside>
</template>

<script>
export default {
  name: 'Aside'
  /* data () {
  } */
}
</script>

<style scoped>
/* min-width: 1125px max-width: 1125px */
@media (min-width: 1126px) {
  aside{
    position: fixed;
    top: 0;
    left: 0;
    width: 300px;
    height: 100vh;
    background: linear-gradient(180deg, #607d8b 0, #212121 100%);
    display: flex;
    flex-direction: column;
    align-items: center;
    user-select: none;
  }
  aside img {
    margin-top: 40px;
  }
  aside > .name {
    margin-top: 40px;
  }
  aside > .motto {
    margin: 30px 0;
  }
  svg {
    font-size: 36px;
    margin: 0 10px;
  }
  aside > .icons {
    font-size: 36px;
  }
  aside > .link {
    display: flex;
    flex-direction: column;
    align-items: center;
  }
  aside > .link > .inside {
    font-size: 16px;
    margin-bottom: 20px;
  }
  aside > .small,aside > .big{
    display: none;
  }
}
@media (max-width: 1125px) {
  aside {
    height: 50px;
    background: linear-gradient(180deg, #607d8b 0, #212121 100%);
    display: flex;
    flex-direction: row;
    align-items: center;
    position: relative;
  }
  aside > span {
    color: #fafafa;
    font-size: 16px;
    padding: 0 1em;
  }
  aside > .big {
    display: inline;
  }
  aside > .small {
    display: none;
  }
  .name,img,.motto,svg,.icons {
    display: none;
  }
  aside > .link {
    position: absolute;
    top: 10px;
    right: 1em;
    font-size: 14px;
    display: flex;
  }
  aside > .link > .inside {
    width: 12vw;
    text-align: center;
    padding: 5px 0;
    border: 1px solid #607d8b;
  }
}
@media (max-width: 768px) {
  aside > .big {
    display: none;
  }
  aside > .small {
    display: inline;
    font-size: 14px;
  }
}

aside > img {
  border: 5px solid #fff;
  border-radius: 50%;
  width: 120px;
}
aside > .name {
  font-family: Roboto, serif;
  font-size: 30px;
  color: #fafafa;
}
aside > .motto {
  font-size: 14px;
  color: #fafafa;
}
aside > .link > .inside > a:hover {
  color: #8bc4e1;
}
aside > .link > .inside > .router-link-exact-active {
  color: #f9c427;
}
</style>
