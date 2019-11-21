<template>
  <main>
    <div class="main">
      <div class="wrap">
        <span class="ribbon6">专业技能</span>
      </div>
      <h2>专业技能</h2>
      <div class="line"></div>
      <h3>技能雷达图</h3>
      <div id="main" style="width: 400px;height: 260px;"></div>
      <h3>技能描述</h3>
      <ul>
        <li><p>在校期间主修的专业课程有VC 程序设计、JAVA 程序设计、计算机网络、SQL 网络数据库、WEB 语言设计基础等。</p></li>
        <li><p>熟练掌握HTML(5)和常用CSS(3)，掌握常用的布局，能够完成界面整洁、交互友好的网页，高度还原UI视觉稿。</p></li>
        <li><p>熟悉原生JavaScript，掌握重要概念如：this、原型、闭包、继承、面向对象等。了解 jQuery 常用 API 及思想。熟练使用ES6及ES7 部分新特性。</p></li>
        <li><p>熟悉 Vue 框架及相关流行库的使用，理解重要概念如：生命周期、组件、数据响应式等。</p></li>
        <li><p>了解小程序开发及相关概念，有相关开发配置经验。 </p></li>
        <li><p>了解HTTP基础知识，了解常见的前端性能优化策略。</p></li>
        <li><p>掌握常用的Git命令，掌握GitHub的基本用法。</p></li>
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
  align-self: center;
}
ul {
  margin: 0;
}
</style>
