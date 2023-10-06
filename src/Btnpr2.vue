<template>
  <a-space direction="vertical" :style="{ width: '100%' }" :size="[0, 48]">
    <a-layout>
      <a-layout-header :style="headerStyle">Header</a-layout-header>
      <a-layout-content :style="contentStyle">Content</a-layout-content>
      <a-layout-footer :style="footerStyle">Footer</a-layout-footer>
    </a-layout>

    <a-layout>
      <a-layout-header :style="headerStyle">Header</a-layout-header>
      <a-layout>
        <a-layout-sider :style="siderStyle">Sider</a-layout-sider>
        <a-layout-content :style="contentStyle">Content</a-layout-content>
      </a-layout>
      <a-layout-footer :style="footerStyle">Footer</a-layout-footer>
    </a-layout>

    <a-layout>
      <a-layout-header :style="headerStyle">Header</a-layout-header>
      <a-layout>
        <a-layout-content :style="contentStyle">Content</a-layout-content>
        <a-layout-sider :style="siderStyle">Sider</a-layout-sider>
      </a-layout>
      <a-layout-footer :style="footerStyle">Footer</a-layout-footer>
    </a-layout>

    <a-layout>
      <a-layout-sider :style="siderStyle">Sider</a-layout-sider>
      <a-layout>
        <a-layout-header :style="headerStyle">Header</a-layout-header>
        <a-layout-content :style="contentStyle">Content</a-layout-content>
        <a-layout-footer :style="footerStyle">Footer</a-layout-footer>
      </a-layout>
    </a-layout>
  </a-space>



  <a-layout class="layout">
    <a-layout-header>
      <div class="logo"/>
      <a-menu
        v-model:selectedkeys="selectedkeys"
        theme="dark"
        mode="horizontal"
        :style="{ linegHeight: '80px'}"
      >
        <a-menu-item key="1">nav 1</a-menu-item>
        <a-menu-item key="2">nav 2</a-menu-item>
        <a-menu-item key="3">nav 3</a-menu-item>
      </a-menu>
    </a-layout-header>
    <a-layout-content style="padding: 0 40px">
      <a-breadcrumb style="margin: 20px 0">
        <a-breadcrumb-item>Home</a-breadcrumb-item>
        <a-breadcrumb-item>List</a-breadcrumb-item>
        <a-breadcrumb-item>App</a-breadcrumb-item>
      </a-breadcrumb>
    <div :style="{ background: '#fff', padding: '24px', minHeight: '280px'}">content</div>
    </a-layout-content>
    <a-layout-footer style="text-align: center">
      앤트디자인 2018년에 만들어짐
    </a-layout-footer>
  </a-layout>
</template>
















<script lang="ts" setup>
import { ref } from 'vue';
import type { CSSProperties } from 'vue';

const selectedkeys = ref<string[]>(['2']);
const headerStyle: CSSProperties = {
  textAlign: 'center',
  color: '#fff',
  height: 64,
  paddingInline: 50,
  lineHeight: '64px',
  backgroundColor: '#7dbcea',
};

const contentStyle: CSSProperties = {
  textAlign: 'center',
  minHeight: 120,
  lineHeight: '120px',
  color: '#fff',
  backgroundColor: '#108ee9',
};

const siderStyle: CSSProperties = {
  textAlign: 'center',
  lineHeight: '120px',
  color: '#fff',
  backgroundColor: '#3ba0e9',
};

const footerStyle: CSSProperties = {
  textAlign: 'center',
  color: '#fff',
  backgroundColor: '#7dbcea',
};
</script>

<style scoped>
.site-layout-content {
  min-height: 280px;
  padding: 24px;
  background: #fff;
}

#components-layout-demo-top .logo {
  float: left;
  width: 120px;
  height: 31px;
  margin: 16px 24px 16px 0;
  background: rgba(255, 255, 255, 0.3);
}

.ant-row-rtl #components-layout-demo-top .logo {
  float: right;
  margin: 16px 0 16px 24px;
}

[data-theme='dark'] .site-layout-content {
  background: #141414;
}


</style>