<script setup lang="ts">
import AppNavi, { MenuItem } from "./components/AppNavi.vue";

// メニューを設定する。
const menuItems: MenuItem[] = [
  {
    type: "heading",
    title: "[Main]",
  },
  {
    type: "menu",
    title: "ToDo",
    icon: "fa-list",
    url: "/todo",
  },
  {
    type: "menu",
    title: "About",
    icon: "fa-list",
    url: "/about",
  },
];
</script>

<template>
  <!-- コンポーネントの利用、タグみたいに使える -->
  <AppNavi title="Todo App" :menu-items="menuItems"></AppNavi>
</template>