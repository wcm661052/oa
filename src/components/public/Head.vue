<template>
  <div class="head">
    <div class="oa-wrap clearfix">
      <a class="fl" href="javascript: void(0)"><img src="../../assets/logo.png"/></a>
      <span class="fl head-title">F2M物联网营商（新运营）应用系统</span>
      <div class="fl">
        <ul class="menu">
          <li>
            <i></i><span>我的桌面</span>
          </li>
          <li>
            <i></i><span>岗位职责</span>
          </li>
          <li>
            <i></i><span>新建任务</span>
          </li>
          <li @click="goIBSS">
            <i></i><span>IBSS</span>
          </li>
          <li @click="goERP">
            <i></i><span>ERP</span>
          </li>
        </ul>
      </div>
    </div>
  </div>
</template>

<script>
  export default {
    name: 'apphead', // Do not use built-in or reserved HTML elements as component id
    data () {

    },
    methods: {
      goIBSS () {
        window.open("http://oms.wm-iot.com/main");
      },
      goERP () {

      }
    }
  }
</script>

<style>
  .head{width: 100%;  height: 100px;  border-bottom: 2px solid rgba(28,30,44,.8);  background: #2a2933;line-height: 100px;}
  .head-title{font-size: 24px;color: #f0f0f0;margin:0 30px;}
  .menu{margin-top: 30px;}
  .menu li{float: left;
    width: 118px;
    height: 40px;
    border-radius: 20px;
    color: #ffffff;
    background: #545266;
    margin-right: 20px;
    font-size: 14px;
    display: flex;
    align-items: center;
    cursor: pointer;}
</style>
