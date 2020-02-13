<template>
  <div id="app" >
    <div class="header">
      <div class="logo">渡一教育</div>
      <ul class="nav">
        <router-link tag="li" to="/">首页</router-link>
        <router-link tag="li" to="/class">课程学习</router-link>
        <router-link tag="li" to="/studentsShow">学员展示</router-link>
        <router-link tag="li" to="/aboutWe">关于</router-link>
        <router-link tag="li" to="/community">社区</router-link>
      </ul>
    </div>
    <router-view class="view"></router-view>
  </div>
</template>

<style scoped>
.header {
  display: flex;
  justify-content: space-between;
  padding: 0 200px;
  background-color: #38f;
  line-height: 70px;
  padding-bottom: 2px;
  color: #fff;
}

.logo {
  cursor: pointer;
}

.nav {
  display: flex;
}

.nav li {
  margin: 0 20px;
  cursor: pointer;
}

.view {
  padding: 50px 200px;
}

.exactActive {
  font-weight: bold;
}
</style>
