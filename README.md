<div align="center">
  
# ⚡ GIT DATA: FRONTEND ⚡
### *Visual Intelligence & Hacker Aesthetic*

[![Vue 3](https://img.shields.io/badge/Framework-Vue%203-42b883?style=for-the-badge&logo=vue.js)](https://vuejs.org/)
[![PrimeVue](https://img.shields.io/badge/UI_Kit-PrimeVue-339af0?style=for-the-badge&logo=primevue)](https://primevue.org/)
[![TypeScript](https://img.shields.io/badge/Language-TypeScript-3178C6?style=for-the-badge&logo=typescript)](https://www.typescriptlang.org/)
[![Vite](https://img.shields.io/badge/Build-Vite-646CFF?style=for-the-badge&logo=vite)](https://vitejs.dev/)

<br />

[![Frontend Repo](https://img.shields.io/badge/Repository-Frontend-42b883?style=flat-square&logo=github)](https://github.com/agussantinelli/GitData-FrontEnd)
[![Backend Repo](https://img.shields.io/badge/Repository-Backend-E0234E?style=flat-square&logo=github)](https://github.com/agussantinelli/GitData-BackEnd)

**GitData-FrontEnd** es la interfaz de asalto de Git Data. Diseñada con una estética *dark-neon* y optimizada para la visualización de datos complejos del ADN de desarrolladores a través de una experiencia inmersiva.

</div>

---

## 🚀 La Experiencia de Usuario (UX)
Este cliente no solo consume datos, los interpreta. Implementa el **Radar de ADN** y el **Timeline de Evolución** mediante componentes reactivos de alto rendimiento, traduciendo JSONs complejos en visualizaciones estratégicas.

### 🛠 Stack Tecnológico
* **Core:** Vue 3 (Composition API) + TypeScript Estricto.
* **UI/UX:** PrimeVue (Presets personalizados) + SCSS (Neon Theme).
* **Estado:** Pinia para una gestión de datos fluida y reactiva.
* **Gráficos:** ECharts / Chart.js para el mapeo de "The Hidden Gem".
* **Validación:** Zod para esquemas de entrada y tipado seguro.

---

## 🏗️ Estructura del Proyecto
Siguiendo los principios de **Arquitecto Git Data**, separamos estrictamente la UI de la lógica de negocio para maximizar la testabilidad:

```text
src/
├── assets/          # Estilos SCSS (Variables Neón, Mixins & Reset)
├── components/      # UI Atoms & Organisms (PrimeVue Overrides)
├── composables/     # Lógica de Negocio Reutilizable (Business Logic)
├── services/        # Adaptadores para la API (Axios/Fetch)
├── stores/          # Gestión de estado global (Pinia)
└── views/           # Páginas principales (Dashboard, Radar, Search)
