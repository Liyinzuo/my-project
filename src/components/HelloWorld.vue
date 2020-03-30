<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
    <br/>
    <el-button @click="show2 = !show2">点我有惊喜</el-button>

     <div style="display: flex; margin-top: 20px; height: 100px;">
      <transition name="el-zoom-in-center">
        <div v-show="show2" class="transition-box">
          <img src="./../assets/lcnb.jpg" title="沙雕刘畅" height=100% weight=100%>
        </div>
      </transition>
    </div>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  data () {
    return {
      msg: 'Welcome to 刘畅是混蛋.com',
      show2: true
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1, h2 {
  font-weight: normal;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
.transition-box{
  width: 400px;
  height: 400px;
  border: 1px;
}
img{
  max-width: 100%;
  max-height: 100%
}
</style>
