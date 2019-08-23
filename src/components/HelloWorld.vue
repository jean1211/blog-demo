<template>
  <div class="hello">
    <Menu mode="horizontal" :theme="theme1" active-name="1">
      <MenuItem name="1">
      <Icon type="md-home" />
      <a href="http://localhost:8080">首页</a>
      </MenuItem>
      <Submenu name="2">
        <template slot="title">
         <Icon type="ios-ionic" />
          小实验
        </template>
        <MenuGroup title="使用">
          <MenuItem name="3-1">新增和启动</MenuItem>
          <MenuItem name="3-2">活跃分析</MenuItem>
          <MenuItem name="3-3">时段分析</MenuItem>
        </MenuGroup>
        <MenuGroup title="留存">
          <MenuItem name="3-4">用户留存</MenuItem>
          <MenuItem name="3-5">流失用户</MenuItem>
        </MenuGroup>
      </Submenu>
      <Submenu name="3">
        <template slot="title">
          <Icon type="ios-folder-open" />
          分类
        </template>
        <MenuGroup title="使用">
          <MenuItem name="3-1">新增和启动</MenuItem>
          <MenuItem name="3-2">活跃分析</MenuItem>
          <MenuItem name="3-3">时段分析</MenuItem>
        </MenuGroup>
        <MenuGroup title="留存">
          <MenuItem name="3-4">用户留存</MenuItem>
          <MenuItem name="3-5">流失用户</MenuItem>
        </MenuGroup>
      </Submenu>
     <Submenu name="4">
        <template slot="title">
         <Icon type="md-flower" />
          综合设置
        </template>
        <MenuGroup title="使用">
          <MenuItem name="3-1">新增和启动</MenuItem>
          <MenuItem name="3-2">活跃分析</MenuItem>
          <MenuItem name="3-3">时段分析</MenuItem>
        </MenuGroup>
        <MenuGroup title="留存">
          <MenuItem name="3-4">用户留存</MenuItem>
          <MenuItem name="3-5">流失用户</MenuItem>
        </MenuGroup>
      </Submenu>
    </Menu>
    <img src="../assets/探头花.png" height="70" width="70" style="position:fixed;right:-3px;bottom:70px">  
    <!-- 右下固定伸缩图标 -->
    <div class="slide">
      <img src="../assets/探头草.png" height="60" width="60">
         <!-- 回到首页 -->
    <div class="back-top">
     <a href="" @click.prevent="top"><i class="ivu-icon ivu-icon-ios-arrow-up" ></i></a>
    </div>
    </div>
         
    <img src="../assets/背景图.jpeg" height="500" width="100%">
    <Button type="primary">1111</Button>
    <a href="" id="top"><p>看完</p></a>
    <p>1</p>
    <p>1</p>
    <p>1</p>
    <p>1</p>
    <p>1</p>
    <p>1</p>
    <p>1</p>
    <p>1</p>
    <p>1</p>
    <p>1</p>
    <p>1</p>
    <p>1</p>
    <p>1</p>
    <p>1</p>
    <p>1</p>
    <p>1</p>
    <p>1</p>
    <p>1</p>
    <p>1</p>
    <p>1</p>
    <p>1</p>
    <p>1</p>
    <p>1</p>
    <p>1</p>
    <p>1</p>
    <p>1</p>
    <p>1</p>
    <p>1</p>
    <p>1</p>
    <p>1</p>
    <p>1</p>
  </div>
</template>
<script>
export default {
  data() {
    return {
      theme1: 'dark',
      scrollTop: 0,
      showTop: false,
      scrollTrigger: false
    }
  },
  name: 'HelloWorld',
  props: {
    msg: String
  },
  methods:{
    top(){
      document.documentElement.scrollTop = document.body.scrollTop = 0
    },
    // enter(){
    //  this.$refs.grass.style.transform = "translate(-60px)"
    // },
    // out(){
    //   this.$refs.grass.style.transform = "translate(0)"
    // }
   
       
    }
  }



</script>
<style scoped lang="less">
.slide{
  display:flex;
  flex-direction:column-reverse;
  position:fixed;
  bottom:0;
  right:0;
  transform:translateX(0px);
  transition:transform 1s ease;
  &:hover{
    transform:translateX(-60px);
    transition:transform 1s ease;
  }
}
ul {
  list-style-type: none;
  width: 100%;
  padding: 0;
  opacity: 0.9;
  background: rgba(40, 42, 44, 0.6);
  position: fixed;
  top: 0;

  a {
    color: rgb(213, 213, 214);

    &:hover {
      color: white;
    }
  }
}

li {
  display: inline-block;
  margin: 0 10px;
}
.back-top{
  width:60px;
  height:42px;
  position:fixed;
  opacity: 0.4;
  background:#9c7b6f;
  bottom:0;
  right:-60px;
  font-size: 20px;
  border-radius:5px;
  i{
    margin:13px;
    color:white;
    &:hover{
      color:black;
    }

  }
}

</style>

