<script lang="ts" setup>
const headerThreeItems = [
  '① 智能择业助你前程无忧',
  '② AI指方向未来不迷茫',
  '③ 精准规划职场快人一步',
  '④ 科学选路事业更成功',
  '⑤ 数据导航就业有保障',
]
const headerTwoItems = [
  '① 命运天机一键知晓未来',
  '② 智能占卜解开人生谜题',
  '③ 科技算命精准预测吉凶',
  '④ 未来运势AI为你揭秘',
  '⑤ 算法知命助你趋吉避凶',
]

const  hotSearchItems = [
  '① AI填志愿助你金榜题名',
  '② 智能选专业前程更无忧',
  '③ 高考择校AI精准指方向',
  '④ 科学选志愿圆梦好大学',
  '⑤ 数据算未来志愿不迷茫',
]


</script>

<template>
  <div class="container">
    <div class="header">
      <div class="bg-primary rounded-50%">
        <div class="size-60 bg-white i-my-svg:system-logo"></div>
      </div>
      <div class="header-text">
        <h1 class="header-title">你的奶油人生助手</h1>
      </div>
    </div>
    <div class="content">
      <div class="card-one">
        <h4 class="title">命理八字</h4>
        <ul>
          <li
            v-for="(item, index) in headerTwoItems"
            :key="index"
            class="list-item"
          >
            {{ item }}
          </li>
        </ul>
      </div>
      <div class="card-two">
        <h4 class="title">高考志愿</h4>
        <ul>
          <li
            v-for="(item, index) in hotSearchItems"
            :key="index"
            class="list-item"
          >
            {{ item }}
          </li>
        </ul>
      </div>
      <div class="card-three">
        <h4 class="title">指点迷津</h4>
        <ul>
          <li
            v-for="(item, index) in headerThreeItems"
            :key="index"
            class="list-item"
          >
            {{ item }}
          </li>
        </ul>
      </div>
    </div>
  </div>
</template>

<style scoped>
body {
  font-family: Arial, sans-serif;
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

.container {
  width: 100%;
  max-width: 900px;
  margin: 0 auto;
  padding: 20px;
}

.header {
  background-color: #f6f7fb;

  /* background: linear-gradient(to right, #f1f0fe, #f3f2ff); */

  border-radius: 5px;
  text-align: center;
  display: flex;
  align-items: center;
  gap: 16px;
  margin-top: 6%;
  justify-content: center;
  padding: 15px;
}

.header-text {
  flex: 1;
  text-align: left;
  flex-grow: 1;
}

.header-title {
  margin: 0; /* Remove default margin */
  font-size: 1.5em; /* Adjust as needed */
}

.header-subtitle {
  margin: 0; /* Remove default margin */
  font-size: 1em; /* Adjust as needed */
  margin-top: 3px; /* Add a small top margin for spacing between title and subtitle */
}

.header > div {
  text-align: left;
}

.content {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 20px;
  margin-top: 10px;
}

.card-one {
  border-radius: 10px;
  padding: 20px;
  background: linear-gradient(to bottom, #f0effe, #d4eefc);
}

.card-two {
  border-radius: 10px;
  padding: 20px;
  background: linear-gradient(to right, #f0effe, #d4eefc);
}

.card-three {
  border-radius: 10px;
  padding: 20px;
  background: linear-gradient(to left, #f0effe, #d4eefc);
}

.card-subtitle {
  margin: 0; /* Remove default margin */
  font-size: 13px; /* Adjust as needed */
  color: #6c757d; /* Optional: to match the color of .header-subtitle */
}

.title {
  color: #333;
  font-size: 17px;
  margin-bottom: 5px;
}

.list-item {
  list-style-type: none;
  margin-bottom: 20px;
  margin-top: 10px;
}
</style>
