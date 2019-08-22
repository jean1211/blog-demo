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
    <img src="../assets/探头草.png" height="100" width="100" style="position:fixed;right:-29px;bottom: -13px">
    <div class="back-top">
     <a href="javascript:scroll(0,0)"><i class="ivu-icon ivu-icon-ios-arrow-up" ></i></a>
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
      theme1: 'dark'
    }
  },
  name: 'HelloWorld',
  props: {
    msg: String
  }
}

</script>
<style scoped lang="less">
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
  height:60px;
  position:fixed;
  opacity: 0.9;
  background:#48484e;
  bottom:0;
  font-size: 20px;
  border-radius:6px;
  i{
    margin:22px 14px;
    color:white;

  }
}

</style>

