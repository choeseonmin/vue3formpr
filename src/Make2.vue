<script lang="ts" setup>
import { reactive, ref, watch } from "vue";
import type { FormInstance } from 'ant-design-vue';

interface FormState {
  username: string;
  nickname: string;
  checkNick: boolean;
}

const formRef = ref<FormInstance>();
const formState = reactive<FormState>({
  username:'',
  nickname:'',
  checkNick:false
});

watch(
    () => formState.checkNick,
    () => {
      formRef.value.validateFields(['nickname']);
    },
    {flush: 'post'},
);

const onCheck = async () => {
  try {
    const values = await formRef.value.validateFields();
    console.log('Success:', values);
  } catch (errorInfo) {
    console.log('Falied:', errorInfo);
  }
};

const formItemLayout = {
  labelCol: { span : 10 },
  wrapperCol: { span: 10},
};

const formTailLayout = {
  labelCol: { span: 4 },
  wrapperCol: { span: 10, offset: 8},
}
</script>

<template>
  <a-form ref="formRef" :model="formState" name="dynamic_rule" v-bind="formItemLayout">
    <a-form-item
      label="Username"
      name="username"
      :rules="[{ required: true, message: '아이디를 입력해주세요!'}]">
      <a-input v-model:value="formState.username"/>
    </a-form-item>

    <a-form-item
        label="Nickname"
        name="nickname"
    :rules="[{ required: true, formState, message: '닉네임을 입력해주세요!' }]">
      <a-input v-model:value="formState.nickname" />
    </a-form-item>

    <a-form-item name="checkNick" v-bind="formTailLayout">
      <a-checkbox v-model:checked="formState.checkNick">중복체크</a-checkbox>
    </a-form-item>

    <a-form-item v-bind="formTailLayout">
      <a-button type="primary" @click="onCheck">Check</a-button>
    </a-form-item>
  </a-form>
</template>

<style scoped>

</style>