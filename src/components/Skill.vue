<template>
  <main>
    <div class="main">
      <div class="wrap">
        <span class="ribbon6">专业技能</span>
      </div>
      <h2>专业技能</h2>
      <div class="line"></div>
      <h3>技能雷达图</h3>
      <div id="main"></div>
      <h3>技能描述</h3>
      <ul>
        <li><p>在校期间主修的 <span class="bold">专业课程</span> 有VC 程序设计、JAVA 程序设计、计算机网络、SQL 网络数据库、WEB 语言设计基础等。</p></li>
        <li><p>熟练掌握 <span class="bold">HTML(5)</span> 和常用 <span class="bold">CSS(3)</span> ，掌握 <span class="bold">常用的布局</span> ，能够完成界面整洁、交互友好的网页，高度还原UI视觉稿。</p></li>
        <li><p>熟悉 <span class="bold">原生JavaScript</span> ，掌握重要概念如：<span class="bold">this、原型、闭包、继承、面向对象</span> 等。了解 jQuery 常用 API 及思想。熟练使用 <span class="bold">ES6及ES7</span> 部分新特性。</p></li>
        <li><p>熟悉 <span class="bold"> Vue 框架</span> 及相关流行库的使用，理解重要概念如：<span class="bold">生命周期、组件、数据响应式</span> 等。</p></li>
        <li><p>了解 <span class="bold">小程序开发</span> 及相关概念，有相关开发配置经验。 </p></li>
        <li><p>了解 <span class="bold">HTTP基础知识</span> ，了解 <span class="bold">常见的前端性能优化</span> 策略。</p></li>
        <li><p>掌握 <span class="bold">常用的Git命令</span> ，掌握GitHub的基本用法。</p></li>
        <!-- <span class="bold"></span> -->
      </ul>
    </div>
  </main>
</template>

<script>
export default {
  name: 'Skill',
  mounted () {
    var myChart = this.$echarts.init(document.getElementById('main'))
    var option = {
      tooltip: {},
      radar: {
        shape: 'circle',
        name: {
          textStyle: {
            color: '#fff',
            backgroundColor: '#999',
            borderRadius: 3,
            padding: [3, 5]
          }
        },
        indicator: [
          {name: 'JavaScript', max: 100},
          {name: 'JQuery', max: 100},
          // {name: 'React', max: 100},
          {name: '小程序', max: 100},
          {name: 'Vue', max: 100},
          {name: 'HTTP', max: 100},
          {name: '移动端页面', max: 100},
          {name: 'HTML/CSS', max: 100}
        ]
      },
      series: [
        {
          name: '预算 vs 开销（Budget vs spending）',
          type: 'radar',
          data: [
            {
              value: [85, 75, 80, 80, 85, 85, 90],
              name: '自我评价'
            }
          ]
        }
      ]
    }
    myChart.setOption(option)
  }
}
</script>

<style scoped>
.main > h2 {
  user-select: none;
}
.main > .line {
  width: 120px;
}
#main {
  width: 400px;
  height: 260px;
  max-width: 90vw;
  align-self: center;
}
ul {
  margin: 0;
}
span.bold {
  font-weight: bold;
}
</style>
