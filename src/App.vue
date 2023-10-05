<template>
  <a-button type="primary">pk</a-button>
  <a-button>Default Button</a-button>
  <a-button type="dashed">asd</a-button>
  <a-button type="text">asd</a-button>
  <a-button type="link">asdasd</a-button>
  <a-button type="primary">asdas</a-button>
<!--  disabled는 클릭 안됨-->
  <a-button type="primary" disabled>asdasd</a-button>
  <a-button>기본</a-button>
  <a-button disabled>기본(disabled)</a-button>
  <a-button type="dashed">대쉬</a-button>
  <a-button type="dashed" disabled>대시 안됨</a-button>
  <a-button type="text">텍스트</a-button>
  <a-button type="text" disabled>텍스트</a-button>
  <a-button type="link">링크</a-button>
  <a-button type="link" disabled>링크 안됨</a-button>
  <a-button danger>danger</a-button>
  <a-button danger disabled>danger</a-button>
  <a-button type="text" danger>danger 텍스트</a-button>
  <a-button type="text" danger disabled>danger 텍스트</a-button>
  <a-button type="link" danger>링크 danger</a-button>
  <a-button type="link" danger disabled>링크 danger</a-button>
  <div :style="{ padding: '8px 8px 0 8px', background: 'rgb(190, 200, 200)' }">
    <a-button ghost>고스트</a-button>
    <a-button ghost disabled>고스트</a-button>
  </div>



</template>

<script setup>
</script>