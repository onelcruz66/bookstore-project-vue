<script setup lang="ts">
import { provide } from "vue";
import { CategoryItem } from "@/types";
import AppHeader from "@/components/AppHeader.vue";
import AppFooter from "@/components/AppFooter.vue";
const categoryList: CategoryItem[] = [
  { categoryId: 1001, name: "Low Fantasy" },
  { categoryId: 1002, name: "High Fantasy" },
  { categoryId: 1003, name: "Sword & Magic" },
  { categoryId: 1004, name: "Dark Fantasy" },
  { categoryId: 1005, name: "Fairy Tales" },
  { categoryId: 1006, name: "Fables" },
];
provide("categoryList", categoryList);
</script>

<style></style>

<template>
  <div id="app">
    <app-header></app-header>
    <router-view></router-view>
    <app-footer></app-footer>
  </div>
</template>
