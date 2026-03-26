<div align="center">

<h1 align="center">⚡ Git Data – FrontEnd</h1>

<p align="center">
  <a href="https://github.com/agussantinelli/GitData-FrontEnd" target="_blank" style="text-decoration: none;">
    <img src="https://img.shields.io/badge/💻%20Repo%20Frontend-GitData-0b7285?style=for-the-badge&logo=github&logoColor=white" alt="Repo Frontend"/>
  </a>
  <a href="https://github.com/agussantinelli/GitData-BackEnd" target="_blank" style="text-decoration: none;">
    <img src="https://img.shields.io/badge/⚙️%20Repo%20Backend-NestJS%20%7C%20Node-E0234E?style=for-the-badge&logo=nestjs&logoColor=white" alt="Repo Backend"/>
  </a>
</p>

<p align="center">
  <a href="https://github.com/agussantinelli" target="_blank" style="text-decoration: none;">
    <img src="https://img.shields.io/badge/👤%20Agustín%20Santinelli-agussantinelli-000000?style=for-the-badge&logo=github&logoColor=white" alt="Agus"/>
  </a>
  <a href="https://github.com/martin-ratti" target="_blank" style="text-decoration: none;">
    <img src="https://img.shields.io/badge/👤%20Martín%20Ratti-martin--ratti-000000?style=for-the-badge&logo=github&logoColor=white" alt="Martín"/>
  </a>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Vue%203-42b883?style=for-the-badge&logo=vue.js&logoColor=white" alt="Vue Badge"/>
  <img src="https://img.shields.io/badge/Vite-6.0.0-646CFF?style=for-the-badge&logo=vite&logoColor=white" alt="Vite Badge"/>
  <img src="https://img.shields.io/badge/TypeScript-5.0.0-3178C6?style=for-the-badge&logo=typescript&logoColor=white" alt="TS Badge"/>
  <img src="https://img.shields.io/badge/PrimeVue-4.0.0-339af0?style=for-the-badge&logo=primevue&logoColor=white" alt="PrimeVue Badge"/>
  <img src="https://img.shields.io/badge/Pinia-2.1.0-ffe14d?style=for-the-badge&logo=pinia&logoColor=black" alt="Pinia Badge"/>
  <img src="https://img.shields.io/badge/Vitest-3.0.0-6E9F18?style=for-the-badge&logo=vitest&logoColor=white" alt="Vitest Badge"/>
  <img src="https://img.shields.io/badge/ESLint-9.0.0-4B32C3?style=for-the-badge&logo=eslint&logoColor=white" alt="ESLint Badge"/>
  <img src="https://img.shields.io/badge/ECharts-Charts-ff6e76?style=for-the-badge&logo=apacheecharts&logoColor=white" alt="ECharts Badge"/>
</p>

**GitData-FrontEnd** es la interfaz de asalto de Git Data. Diseñada con una estética *dark-neon* y optimizada para la visualización de datos complejos del ADN de desarrolladores a través de una arquitectura limpia y reactiva.

</div>

---

## 🎯 Objetivo y Propósito

### El "Por Qué" de Git Data
En un ecosistema saturado de métricas vanidosas (como el número de contribuciones o "streaks"), los reclutadores y líderes técnicos a menudo pierden de vista el **impacto real** y la **calidad técnica** de un desarrollador. 

**Git Data** nace para resolver la opacidad en el análisis de perfiles de GitHub, transformando datos crudos en una radiografía técnica precisa.

### Objetivos Estratégicos
* **🔍 Análisis de ADN Técnico:** Desglosar el stack real de un usuario basándose en la complejidad de sus repositorios, no solo en sus lenguajes más usados.
* **💎 The Hidden Gem (La Joya Oculta):** Algoritmo diseñado para identificar repositorios con alto valor técnico o arquitectónico que suelen quedar enterrados por proyectos menores.
* **📊 Visualización de Alto Impacto:** Sustituir tablas aburridas por un **Radar de Competencias** y **Timelines de Evolución** interactivos, permitiendo una toma de decisiones basada en datos (Data-Driven).
* **🚀 Optimización de Reclutamiento:** Reducir el tiempo de revisión de perfiles técnicos mediante un resumen ejecutivo generado por inteligencia analítica.

> **Propósito Final:** Empoderar a la comunidad dev y a los Tech-Recruiters con una herramienta de auditoría técnica que premie la calidad, la consistencia y la arquitectura sobre el simple volumen de código.

---

## 🚀 La Experiencia de Usuario (UX)
Este cliente no solo consume datos, los interpreta. Implementa el **Radar de ADN** y el **Timeline de Evolución** mediante componentes reactivos de alto rendimiento, traduciendo JSONs complejos en visualizaciones estratégicas.

### 🛠 Stack Tecnológico
* **Core:** Vue 3 (Composition API) + TypeScript Estricto.
* **UI/UX:** PrimeVue (Presets personalizados) + SCSS (Neon Theme).
* **Estado:** Pinia para una gestión de datos fluida y reactiva.
* **Gráficos:** ECharts para el mapeo de "The Hidden Gem".
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
