---
name: integration-testing
description: Guidelines for frontend integration testing using Vitest and Vue Test Utils for GitData.
---

# 🔗 GitData Integration Testing

Integration tests in the GitData FrontEnd focus on the interaction between multiple components, Pinia stores, and services. They verify that our "Technical Data Sheet" components (Radar, Timeline, etc.) work together correctly.

## 🛠️ Stack
- **Framework**: [Vitest](https://vitest.dev/)
- **Library**: [@vue/test-utils](https://test-utils.vuejs.org/)
- **Environment**: `happy-dom`
- **Mocking**: `vi.mock()` for API services.

## 📂 Location
`src/**/__tests__/*.spec.ts` or `src/tests/integration/*.spec.ts`.

## 📏 Core Principles
1. **State Integration**: Test components with their real **Pinia** stores. Use `createTestingPinia()` to pre-fill state if needed.
2. **Service Interaction**: Verify that components correctly trigger service calls (e.g., fetching GitHub data).
3. **Data Flows**: Focus on critical "GitData Pro" flows:
    - User search triggering the profile load.
    - Radar interaction highlighting specific repositories.
    - Switch Mode (Reclutador/Developer) changing the UI perspective.
4. **No Real API**: Always mock the backend responses to ensure deterministic tests.

## 🧪 Example (Vue + Pinia)
```typescript
import { mount } from '@vue/test-utils'
import { createTestingPinia } from '@pinia/testing'
import ProfileDashboard from '@/views/ProfileDashboard.vue'

it('should display the radar when profile data is loaded', async () => {
    const wrapper = mount(ProfileDashboard, {
        global: {
            plugins: [createTestingPinia({
                initialState: { profile: { data: mockProfile } }
            })]
        }
    })
    
    expect(wrapper.findComponent({ name: 'RadarChart' }).exists()).toBe(true)
})
```
