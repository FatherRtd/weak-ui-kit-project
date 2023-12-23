<script setup lang="ts">
import WButton from "@/components/button/WButton.vue";
import WText from "@/components/text/WText.vue";
import WTag from "@/components/tag/WTag.vue";
import WLink from "@/components/link/WLink.vue";
import WInput from "@/components/input/WInput.vue";
import { ref } from "vue";

const textInput = ref<string>("");
</script>

<template>
  <div>
    <h1>Кнопка</h1>
    <div class="items-row">
      <h2>Тип</h2>
      <WButton>button</WButton>
      <WButton type="primary">button</WButton>
      <WButton type="success">button</WButton>
      <WButton type="danger">button</WButton>
      <WButton type="warning">button</WButton>
    </div>
    <div class="items-row">
      <h2>Круглые</h2>
      <WButton round>button</WButton>
      <WButton type="primary" round>button</WButton>
      <WButton type="success" round>button</WButton>
      <WButton type="danger" round>button</WButton>
      <WButton type="warning" round>button</WButton>
    </div>
    <div class="items-row">
      <h2>Выключены</h2>
      <WButton disabled>button</WButton>
      <WButton type="primary" disabled>button</WButton>
      <WButton type="success" disabled>button</WButton>
      <WButton type="danger" disabled>button</WButton>
      <WButton type="warning" disabled>button</WButton>
    </div>
    <div class="items-row">
      <h2>Большие</h2>
      <WButton size="large">button</WButton>
      <WButton type="primary" size="large">button</WButton>
      <WButton type="success" size="large">button</WButton>
      <WButton type="danger" size="large">button</WButton>
      <WButton type="warning" size="large">button</WButton>
    </div>
    <div class="items-row">
      <h2>Средние</h2>
      <WButton size="small">button</WButton>
      <WButton type="primary" size="small">button</WButton>
      <WButton type="success" size="small">button</WButton>
      <WButton type="danger" size="small">button</WButton>
      <WButton type="warning" size="small">button</WButton>
    </div>
    <div class="items-row">
      <h2>Мальенькие</h2>
      <WButton size="mini">button</WButton>
      <WButton type="primary" size="mini">button</WButton>
      <WButton type="success" size="mini">button</WButton>
      <WButton type="danger" size="mini">button</WButton>
      <WButton type="warning" size="mini">button</WButton>
    </div>
    <div class="items-row">
      <h2>Прямоугольные</h2>
      <WButton square>button</WButton>
      <WButton type="primary" square>button</WButton>
      <WButton type="success" square>button</WButton>
      <WButton type="danger" square>button</WButton>
      <WButton type="warning" square>button</WButton>
    </div>
    <div class="items-row">
      <h2>Упрощённый тип</h2>
      <WButton simple>button</WButton>
      <WButton type="primary" simple>button</WButton>
      <WButton type="success" simple>button</WButton>
      <WButton type="danger" simple>button</WButton>
      <WButton type="warning" simple>button</WButton>
    </div>
  </div>

  <div>
    <h1>Текст</h1>
    <div class="items-row">
      <h2>Тип</h2>
      <WText>text</WText>
      <WText type="primary">text</WText>
      <WText type="success">text</WText>
      <WText type="danger">text</WText>
      <WText type="warning">text</WText>
    </div>
  </div>

  <div>
    <h1>Тэг</h1>
    <div class="items-row">
      <h2>Тип</h2>
      <WTag>tag</WTag>
      <WTag type="primary">tag</WTag>
      <WTag type="success">tag</WTag>
      <WTag type="danger">tag</WTag>
      <WTag type="warning">tag</WTag>
    </div>

    <div class="items-row">
      <h2>Круглые</h2>
      <WTag round>tag</WTag>
      <WTag type="primary" round>tag</WTag>
      <WTag type="success" round>tag</WTag>
      <WTag type="danger" round>tag</WTag>
      <WTag type="warning" round>tag</WTag>
    </div>

    <div class="items-row">
      <h2>Средние</h2>
      <WTag size="small">tag</WTag>
      <WTag type="primary" size="small">tag</WTag>
      <WTag type="success" size="small">tag</WTag>
      <WTag type="danger" size="small">tag</WTag>
      <WTag type="warning" size="small">tag</WTag>
    </div>

    <div class="items-row">
      <h2>Маленькие</h2>
      <WTag size="mini">tag</WTag>
      <WTag type="primary" size="mini">tag</WTag>
      <WTag type="success" size="mini">tag</WTag>
      <WTag type="danger" size="mini">tag</WTag>
      <WTag type="warning" size="mini">tag</WTag>
    </div>
  </div>

  <div>
    <h1>Ссылка</h1>
    <div class="items-row">
      <h2>Тип</h2>
      <WLink>link</WLink>
      <WLink type="primary">link</WLink>
      <WLink type="success">link</WLink>
      <WLink type="danger">link</WLink>
      <WLink type="warning">link</WLink>
    </div>

    <div class="items-row">
      <h2>Подчёркивание</h2>
      <WLink :underline="false">link</WLink>
      <WLink type="primary" :underline="false">link</WLink>
      <WLink type="success" :underline="false">link</WLink>
      <WLink type="danger" :underline="false">link</WLink>
      <WLink type="warning" :underline="false">link</WLink>
    </div>

    <div class="items-row">
      <h2>Выключена</h2>
      <WLink isdisable>link</WLink>
      <WLink type="primary" isdisable>link</WLink>
      <WLink type="success" isdisable>link</WLink>
      <WLink type="danger" isdisable>link</WLink>
      <WLink type="warning" isdisable>link</WLink>
    </div>
  </div>

  <div>
    <h1>Поле ввода</h1>
    <div class="items-row">
      <h2>Простой ввод</h2>
      <WInput v-model="textInput" />
    </div>
  </div>
</template>

<style scoped>
.items-row {
  display: flex;
  align-items: center;
  gap: 1rem;
}
</style>

