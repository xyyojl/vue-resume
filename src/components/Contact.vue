<template>
  <main>
    <div class="main">
      <div class="wrap">
        <span class="ribbon6">联系方式</span>
      </div>
      <h2>联系我</h2>
      <p class="title">
        本人是 2020 届五邑大学信息管理与信息系统专业的本科应届毕业生，正在寻求一份前端工程师的工作，如蒙青睐，不胜荣幸。
      </p>
      <p class="way">
        <svg class="icon" aria-hidden="true">
          <use xlink:href="#icon-tel"></use>
        </svg> 13631897256
      </p>
      <p class="way">
        <svg class="icon" aria-hidden="true">
          <use xlink:href="#icon-wechat"></use>
        </svg> 13631897256
      </p>
      <p class="way">
        <svg class="icon" aria-hidden="true">
          <use xlink:href="#icon-email"></use>
        </svg> m13631897256@163.com
      </p>
    </div>
  </main>
</template>

<script>
export default {
  name: 'Contact'
}
</script>

<style scoped>
.main > .line {
  width: 60px;
}
p.way {
  display: flex;
  align-items: center;
  font-size: 30px;
  margin: .4em;
  font-weight: bold;
  color: #333;
}
svg {
  margin-right: 10px;
}
@media (max-width: 550px) {
  p.way{
    font-size: 20px;
  }
  .main {
    min-height: 85vh;
  }
}
</style>
