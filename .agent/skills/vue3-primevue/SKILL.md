---
name: vue3-primevue
description: Mandatory rules for Vue 3 (Composition API), PrimeVue 4, and Neon Styling.
---

# ⚡ GitData Vue 3 & PrimeVue

Guidelines for building high-performance, stunning UIs for GitData.

## 🟢 Vue 3 (Composition API)
1. **Script Setup**: Always use `<script setup lang="ts">`.
2. **Reactivity**: Use `ref()` for primitives and `reactive()` for objects when appropriate.
3. **Composables**: Extract reusable logic into `src/composables`.

## 🎨 PrimeVue 4 & Styling
1. **Components**: Use PrimeVue components for all UI elements.
2. **Theming**: Follow the "Neon Theme" using SCSS variables in `src/assets`.
3. **Icons**: Use PrimeIcons or the specific icon sets defined in the project.

## 📂 Structure
- `src/components`: UI Atoms and Organisms.
- `src/views`: Page components.
- `src/stores`: Pinia stores for state management.
