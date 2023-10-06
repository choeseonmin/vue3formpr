<script lang="ts" setup>
import type { MenuProps } from 'ant-design-vue';

const data: string[] = [
    'Racing car sprays burning fuel into crowd.',
    'Japanese princess to wed commoner.',
    'Australian walks 100km after outback crash.',
    'Man charged over missing wedding girl',
    'Los Angeles battles huge wildfires',
];

const handleMenuClick: MenuProps['onClick'] = e => {
  console.log('click', e);
};
</script>

<template>
  <a-list style="width: 300%" bordered :data-source="data">
    <template #renderItem="{ item }">
      <a-list-item>{{ item }}</a-list-item>
    </template>
    <template #header>
      <div style="font-size: 20px; margin: 5px">공지사항</div>
      <a-button style="margin: 4px">글 작성</a-button>
      <a-button style="margin: 4px">수정</a-button>
      <a-button style="margin: 4px">삭제</a-button>
    </template>
    <template #footer>
      <div>
        <a-dropdown>
      <template #overlay>
        <a-menu style="margin: 10px" @click="handleMenuClick">
          <a-menu-item key="1">
            <UserOutlined />
            제목
          </a-menu-item>
          <a-menu-item key="2">
            <UserOutlined />
            작성자
          </a-menu-item>
          <a-menu-item key="3">
            <UserOutlined />
            내용
          </a-menu-item>
        </a-menu>
      </template>
      <a-button style="margin: 5px">
        제목
        <DownOutlined />
      </a-button>
    </a-dropdown>
      </div>
    </template>
  </a-list>

</template>


<style scoped>

</style>