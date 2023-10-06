<template xmlns="http://www.w3.org/1999/html">
<!--  <a-button type="primary">pk</a-button>-->
<!--  <a-button>Default Button</a-button>-->
<!--  <a-button type="dashed">asd</a-button>-->
<!--  <a-button type="text">asd</a-button>-->
<!--  <a-button type="link">asdasd</a-button>-->
<!--  <a-button type="primary">asdas</a-button>-->
<!--&lt;!&ndash;  disabled는 클릭 안됨&ndash;&gt;-->
<!--  <a-button type="primary" disabled>asdasd</a-button>-->
<!--  <a-button>기본</a-button>-->
<!--  <a-button disabled>기본(disabled)</a-button>-->
<!--  <a-button type="dashed">대쉬</a-button>-->
<!--  <a-button type="dashed" disabled>대시 안됨</a-button>-->
<!--  <a-button type="text">텍스트</a-button>-->
<!--  <a-button type="text" disabled>텍스트</a-button>-->
<!--  <a-button type="link">링크</a-button>-->
<!--  <a-button type="link" disabled>링크 안됨</a-button>-->
<!--  <a-button danger>danger</a-button>-->
<!--  <a-button danger disabled>danger</a-button>-->
<!--  <a-button type="text" danger>danger 텍스트</a-button>-->
<!--  <a-button type="text" danger disabled>danger 텍스트</a-button>-->
<!--  <a-button type="link" danger>링크 danger</a-button>-->
<!--  <a-button type="link" danger disabled>링크 danger</a-button>-->
<!--  <div :style="{ padding: '8px 8px 0 8px', background: 'rgb(190, 200, 200)' }">-->
<!--    <a-button ghost>고스트</a-button>-->
<!--    <a-button ghost disabled>고스트</a-button>-->
<!--  </div>-->
<!--  <a-space style="width: 100%">-->

<!--&lt;!&ndash;    loading, 로딩은  빙글빙글도는 애니메이션을 추가함&ndash;&gt;-->
<!--      <a-button type="primary" size="small" loading>작은 로딩</a-button>-->
<!--      <a-button type="primary" loading>로딩</a-button>-->
<!--  </a-space>-->
<!--  <a-space style="width: 100%">-->
<!--    <a-button type="primary" :loading="loading" @mouseenter="loading = true">마우스 엔터</a-button>-->
<!--    <a-button type="primary" :loading="iconLoading" @click="enterIconLoading">-->
<!--      <template #icon><PoweroffOutlined /></template>-->
<!--      1초-->
<!--    </a-button>-->
<!--  </a-space>-->
<!--  <a-space style="width: 100%">-->
<!--    <a-button type="primary" loading />-->
<!--    <a-button type="primary" shape="circle" loading/>-->
<!--    <a-button danger shape="round" loading/>-->
<!--    <a-button type="primary" shape="circle">원-->
<!--    <template #icon><SearcOutlined/></template></a-button>-->
<!--    <a-button type="primary" shape="circle>">A</a-button>-->

<!--    <a-button type="primary">-->
<!--    <template #icon><SearchOutlined /></template>-->
<!--    검색-->
<!--  </a-button>-->
<!--  <a-button shape="circle">-->
<!--    <template #icon><SearchOutlined /></template>-->
<!--  </a-button>-->
<!--  <a-button>-->
<!--    <template #icon><SearchOutlined /></template>-->
<!--    검색-->
<!--  </a-button>-->
<!--  <a-button shape="circle">-->
<!--    <template #icon><SearchOutlined /></template>-->
<!--  </a-button>-->
<!--  <a-button>-->
<!--    <template #icon><SearchOutlined /></template>-->
<!--    검색-->
<!--  </a-button>-->
<!--  <a-button type="dashed" shape="circle">-->
<!--    <template #icon><SearchOutlined /></template>-->
<!--  </a-button>-->

<!--    <a-button type="dashed">-->
<!--      <template #icon><SearchOutlined/></template>-->
<!--      검색-->
<!--    </a-button>-->
<!--    <a-button href="https://www.google.com">-->
<!--      <template #icon><SearchOutlined/></template>-->
<!--    </a-button>-->

<!--    <br/>-->
<!--    <br/>-->
<!--&lt;!&ndash;    tooltip, 툴팁은 마우스를 가져고 갔을 때 title이 나옴&ndash;&gt;-->
<!--    <a-tooltip title="search">-->
<!--      <a-button type="primary" shape="circle" size="large">-->
<!--        <template #icon><SearchOutlined/></template>-->
<!--        검색-->
<!--      </a-button>-->
<!--    </a-tooltip>-->

<!--    <a-button type="primary" shape="circle" size="large">A</a-button>-->
<!--    <a-button type="primary" size="large">-->
<!--      <template #icon><Searchoulined/></template>-->
<!--      검색-->
<!--    </a-button>-->

<!--    <a-tooltip title="search">-->
<!--      <a-button shape="circle" size="large">-->
<!--        <template #icon><SearchOutlined/></template>-->
<!--      </a-button>-->
<!--    </a-tooltip>-->
<!--    <a-button size="large">-->
<!--      <template #icon><SearchOutlined/></template>-->
<!--      검색-->
<!--    </a-button>-->
<!--    <br/>-->
<!--    <a-tooltip title="search">-->
<!--      <a-button shape="circle" size="large">-->
<!--        <template #icon><SearchOutlined/></template>-->
<!--      검색-->
<!--      </a-button>-->
<!--    </a-tooltip>-->
<!--    <a-button size="large">-->
<!--      <template><SearchOutlined/></template>-->
<!--      검색-->
<!--    </a-button>-->
<!--    <a-tooltip title="search">-->
<!--      <a-button type="dashed" shape="circle" size="large">-->
<!--        <template #icon><SearchOutlined/></template>-->
<!--      </a-button>-->
<!--    </a-tooltip>-->
<!--    <a-button type="dashed" size="large">-->
<!--      <template #icon><SearchOutlined/></template>-->
<!--    </a-button>-->
<!--  </a-space>-->
  <a-divider>게시글 포함</a-divider>
  <br>
    <p>
      <a-divider>아자아자</a-divider>
    열심히하자
    </p>
  <div>
    text
    <a-divider type="vertical" />
    <a href="#">Link</a>
    <a-divider type="vertical"/>
    <a href="#">Link</a>
  </div>
  <a-row>
    <a-col :span="10">col</a-col>
  </a-row>
  <a-row>
    <a-col :span="12">col-12</a-col>
    <a-col :span="12">col-12</a-col>
  </a-row>
  <a-row>
    <a-col :span="8">col-8</a-col>
    <a-col :span="8">col-8</a-col>
    <a-col :span="8">col-8</a-col>
  </a-row>
  <a-row>
    <a-col :span="6">col-6</a-col>
    <a-col :span="6">col-6</a-col>
    <a-col :span="6">col-6</a-col>
    <a-col :span="6">col-6</a-col>
  </a-row>

  <div>
    <a-divider orientation="left">Horizontal</a-divider>
    <a-row :gutter="16">
      <a-col class="gutter-row" :span="6">
        <div class="gutter-box">col-6</div>
      </a-col>
    <a-col class="gutter-row" :span="6">
      <div class="gutter-box">col-6</div>
    </a-col>
      <a-col class="gutter-row" :span="6">
        <div class="gutter-box">col-6</div>
      </a-col>
      <a-col class="gutter-row" :span="6">
        <div class="gutter-box">col-6</div>
      </a-col>
    </a-row>
    <a-divider orientation="left">Responsive</a-divider>
    <a-row :gutter="{xs:8, sm:16, md:24, lg:32}">
      <a-col class="gutter-row" :span="6">
        <div class="gutter-box">col-6</div>
      </a-col>
       <a-col class="gutter-row" :span="6">
        <div class="gutter-box">col-6</div>
      </a-col>
       <a-col class="gutter-row" :span="6">
        <div class="gutter-box">col-6</div>
      </a-col>
       <a-col class="gutter-row" :span="6">
        <div class="gutter-box">col-6</div>
      </a-col>
    </a-row>
    <a-divider orientation="left">Vertical</a-divider>
    <a-row :gutter="[16,24]">
      <a-col class="gutter-row" :span="6">
      <div class="gutter-box">col-6</div>
    </a-col>
    </a-row>
  </div>
  <div>
  <a-row>
    <a-col :span="8">col 8</a-col>
    <a-col :span="8" :offset="8">col8</a-col>
  </a-row>
    <a-row>
    <a-col :span="6" :offset="6">col 6 col offset 6</a-col>
    <a-col :span="6" :offset="6">col 6 col offset 6</a-col>
    </a-row>
    <a-divider orientation="left">sub-elment align center</a-divider>
    <a-row justify="center">
      <a-col :span="4">col4</a-col>
      <a-col :span="4">col4</a-col>
      <a-col :span="4">col4</a-col>
      <a-col :span="4">col4</a-col>
    </a-row>
  </div>








</template>

<script lang="ts">
import { defineComponent, ref } from 'vue';
import { PoweroffOutlined } from '@ant-design/icons-vue';
import { SearchOutlined } from '@ant-design/icons-vue';

interface DelayLoading {
  delay: number;
}
export default defineComponent({
  components: { PoweroffOutlined },
  setup() {
    const iconLoading = ref<boolean | DelayLoading>(false);
    const enterIconLoading = () => {
      iconLoading.value = { delay: 1000 };

      setTimeout(() => {
        iconLoading.value = false;
      }, 6000);
    };
    return {
      loading: ref(false),
      iconLoading,
      enterIconLoading,
    };
  },
});
</script>


<script setup>
</script>

<style scoped>
  .gutter-box {
    background: #0092ff;
    padding: 8px 0;
  }

</style>
<style lang="less" scoped>
:deep(#components-grid-demo-flex) [class~='ant-row'] {
  background: rgba(128,128,128,0.08);
}
</style>