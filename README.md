
<!-- TOC -->

- [Bootstrap-Vue 基于全球最流行的前端框架组合应用系统](#bootstrap-vue-基于全球最流行的前端框架组合应用系统)
    - [项目介绍](#项目介绍)
    - [相关链接](#相关链接)
    - [快速安装方法](#快速安装方法)
    - [快速使用](#快速使用)
        - [一个快速列偏移栅格示例：](#一个快速列偏移栅格示例)
        - [图片引用方法：](#图片引用方法)
        - [button按钮引用方法：](#button按钮引用方法)
        - [form引用方法:](#form引用方法)
        - [nav头部导航引用：](#nav头部导航引用)
        - [链接：](#链接)
        - [输入框（input Group):](#输入框input-group)
        - [表格用例：](#表格用例)
        - [下拉菜单:](#下拉菜单)
    - [Zoomla!逐浪CMS团队卓越出品](#zoomla逐浪cms团队卓越出品)
    - [翻译日志](#翻译日志)

<!-- /TOC -->


<p align="center">
  <a href="http://code.z01.com/bootstrap-vue">
    <img src="http://code.z01.com/bootstrap-vue/style/icons/icon_512.png" width="300">
  </a>
</p>
<br>


<p align="center">

  <a href="https://www.npmjs.com/package/bootstrap-vue">
    <img src="https://flat.badgen.net/npm/v/bootstrap-vue" alt="Current version">
  </a>
  <a href="https://getbootstrap.com/docs">
    <img src="https://flat.badgen.net/badge/bootstrap/4.3.x/563d7c" alt="Bootstrap version">
  </a>
  <a href="https://vuejs.org">
    <img src="https://flat.badgen.net/badge/vue.js/2.6.x/4fc08d" alt="Vue.js version">
  </a>
  <a href="https://github.com/bootstrap-vue/bootstrap-vue/actions?workflow=Tests">
    <img src="https://flat.badgen.net/github/status/bootstrap-vue/bootstrap-vue" alt="Build status">
  </a>
  <a href="https://github.com/bootstrap-vue/bootstrap-vue">
    <img src="https://flat.badgen.net/david/dep/bootstrap-vue/bootstrap-vue" alt="Dependencies status">
  </a>
  <br>
  <a href="https://codecov.io/gh/bootstrap-vue/bootstrap-vue">
    <img src="https://flat.badgen.net/codecov/c/github/bootstrap-vue/bootstrap-vue" alt="Coverage">
  </a>
  <a href="https://packagequality.com/#?package=bootstrap-vue">
    <img src="https://npm.packagequality.com/shield/bootstrap-vue.svg?style=flat-square" alt="Package quality">
  </a>
  <a href="https://www.npmjs.com/package/bootstrap-vue">
    <img src="https://flat.badgen.net/npm/dt/bootstrap-vue" alt="npm downloads">
  </a>
  <a href="https://www.npmjs.com/package/bootstrap-vue">
    <img src="https://flat.badgen.net/npm/dw/bootstrap-vue" alt="npm monthly downloads">
  </a>
  <br>
  <a href="https://opencollective.com/bootstrap-vue#sponsor">
    <img src="https://opencollective.com/bootstrap-vue/sponsors/badge.svg?style=flat-square" alt="Open Collective sponsors">
  </a>
  <a href="https://opencollective.com/bootstrap-vue#backer">
    <img src="https://flat.badgen.net/opencollective/backers/bootstrap-vue" alt="Open Collective backers">
  </a>
  <a href="https://opencollective.com/bootstrap-vue">
    <img src="https://flat.badgen.net/opencollective/balance/bootstrap-vue" alt="Open Collective balance">
  </a>
</p>

# Bootstrap-Vue 基于全球最流行的前端框架组合应用系统


## 项目介绍
BootstrapVue中文手册，由Bootstrap中文站(http://code.z01.com/v4 ）官方团队翻译支持，一套将全球最流行的前端框架Bootstap与中国最流行的前端webpack库Vue完美结合的框架，精良翻译，服务国人。

Bootstrap是全球最流行的前端框架，基于twitter团队的奉献。
Vue是中国最火的webpack框架。
二者结合，诞生了BootstrapVue项目。

翻译团队：Zoomla!逐浪CMS

## 相关链接

BootStrap-Vue官方站：https://bootstrap-vue.org/

BootStrap-Vue官方Github库：https://github.com/bootstrap-vue/bootstrap-vue

---
BootStrap中文手册官方站：http://code.z01.com/bootstrap-vue

BootStrap中文手册Github官方库：https://github.com/zoomla/bootstrapVue-cn

BootStrap中文手册Gitee官方库：https://gitee.com/zoomla/Bootstrap-Vue



##  快速安装方法 
```
npm i bootstrap-vue
#或者全栈生态
npm install vue bootstrap-vue bootstrap
```

## 快速使用

### 一个快速列偏移栅格示例：
```
<b-container fluid="xl" class="">
   <b-row>
   <b-col md="4" offset="2">left test
   </b-col>
   <b-col md="6">right test
   </b-col>
   </b-row>
</b-container>
```

### 图片引用方法：
```
<b-img src="../assets/images/name.png" alt=""></b-img>
```

### button按钮引用方法：
```
<b-button variant="danger">Button</b-button>

```

### form引用方法:
```
<b-form-input v-model="text" placeholder="Enter your name"></b-form-input>
```


### nav头部导航引用：
```
   <b-navbar toggleable="lg" type="dark" variant="info">
   <b-navbar-brand href="#">NavBar</b-navbar-brand>
   <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>
   <b-collapse id="nav-collapse" is-nav>
       <b-navbar-nav>
       <b-nav-item href="#">Link</b-nav-item>
       <b-nav-item href="#" disabled>Disabled</b-nav-item>
       </b-navbar-nav>
       <b-navbar-nav class="ml-auto">
       <b-nav-form>
       <b-form-input size="sm" class="mr-sm-2" placeholder="Search"></b-form-input>
       <b-button size="sm" class="my-2 my-sm-0" type="submit">Search</b-button>
      </b-nav-form>
      <b-nav-item-dropdown text="Lang" right>
          <b-dropdown-item href="#">EN</b-dropdown-item>
          <b-dropdown-item href="#">CN</b-dropdown-item>
      </b-nav-item-dropdown>
      <b-nav-item-dropdown right>
          <template v-slot:button-content>
          <em>User</em>
          </template>
          <b-dropdown-item href="#">Profile</b-dropdown-item>
          <b-dropdown-item href="#">Sign Out</b-dropdown-item>
      </b-nav-item-dropdown>
      </b-navbar-nav>
   </b-collapse>
   </b-navbar>
```

### 链接：
```
 <b-link href="#foo">Link</b-link>
```

### 输入框（input Group):
```
<div>
  <!-- Using props -->
  <b-input-group size="lg" prepend="$" append=".00">
    <b-form-input></b-form-input>
  </b-input-group>

  <!-- Using slots -->
  <b-input-group class="mt-3">
    <template v-slot:append>
      <b-input-group-text><strong class="text-danger">!</strong></b-input-group-text>
    </template>
    <b-form-input></b-form-input>
  </b-input-group>

  <!-- Using components -->
  <b-input-group prepend="Username" class="mt-3">
    <b-form-input></b-form-input>
    <b-input-group-append>
      <b-button variant="outline-success">Button</b-button>
      <b-button variant="info">Button</b-button>
    </b-input-group-append>
  </b-input-group>
</div>
```

### 表格用例：
```
<template>
  <div>
    <b-table striped hover :items="items"></b-table>
  </div>
</template>

<script>
  export default {
    data() {
      return {
        items: [
          { age: 40, first_name: 'Dickerson', last_name: 'Macdonald' },
          { age: 21, first_name: 'Larsen', last_name: 'Shaw' },
          { age: 89, first_name: 'Geneva', last_name: 'Wilson' },
          { age: 38, first_name: 'Jami', last_name: 'Carney' }
        ]
      }
    }
  }
</script>
```

### 下拉菜单:
```
<div>
  <b-dropdown id="dropdown-1" text="Dropdown Button" class="m-md-2">
    <b-dropdown-item>First Action</b-dropdown-item>
    <b-dropdown-item>Second Action</b-dropdown-item>
    <b-dropdown-item>Third Action</b-dropdown-item>
    <b-dropdown-divider></b-dropdown-divider>
    <b-dropdown-item active>Active action</b-dropdown-item>
    <b-dropdown-item disabled>Disabled action</b-dropdown-item>
  </b-dropdown>
</div>
```
## Zoomla!逐浪CMS团队卓越出品
**CMS+AI智能+字库+图库全栈生态-->做中国最优秀的全栈门户服务商**

Zoomla!逐浪CMS：中文业界alexa排名第一的CMS系统|专注.net与windows平台企业级研发，集成内容管理、webfont、商城、店铺、黄页、教育、考试、3D、三维全景、混合现实、CRM、ERP、OA、论坛、贴吧等为一体，打造国内高端的CMS产品典范。

官网：http://www.z01.com

免费下载：http://www.z01.com/mb

视频教程：http://www.z01.com/mtv

模板资源：http://www.z01.com/mb

zico中文图标库：http://ico.z01.com

Uni全球字码表：http://www.ziti163.com/uni

webfont： http://www.ziti163.com/webfont

字典： http://zd.ziti163.com

在线智写做字库： http://v.ziti163.com

方言语音项目： http://a.ziti163.com

智图： http://p.ziti163.com


QQ交流群号：
[![加入QQ群](https://img.shields.io/badge/一群-541450128-blue.svg?style=for-the-badge&logo=appveyor)](https://jq.qq.com/?_wv=1027&k=5qIayyX)  [![加入QQ群](https://img.shields.io/badge/二群-541450128-blue.svg?style=for-the-badge&logo=appveyor)](https://jq.qq.com/?_wv=1027&k=5Ephzpq)   [![加入QQ群](https://img.shields.io/badge/三群-601781959-blue.svg?style=for-the-badge&logo=appveyor)](https://jq.qq.com/?_wv=1027&k=50a28BK) 


官方QQ客服：
[![官方QQ客服1](https://img.shields.io/badge/官方QQ客服1-524979923-red.svg?style=for-the-badge&logo=appveyor)](http://wpa.qq.com/msgrd?v=3&uin=745151353&site=qq&menu=yes)  [![官方QQ客服2](https://img.shields.io/badge/官方QQ客服2-1799661890-red.svg?style=for-the-badge&logo=appveyor)](http://wpa.qq.com/msgrd?v=3&uin=1799661890&site=qq&menu=yes) 




## 翻译日志
- 20200201 启动翻译
- 20200301 小米立同学加入
- 20200425 正式完成翻译
