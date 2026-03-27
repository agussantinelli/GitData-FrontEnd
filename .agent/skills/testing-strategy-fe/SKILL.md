---
name: testing-strategy-fe
description: Guidelines for frontend testing using Vitest and Vue Test Utils.
---

# 🧪 GitData FrontEnd Testing Strategy

Ensuring "Zero Regression" in the GitData Dashboard.

## 🛠 Tools
1. **Vitest**: Main test runner.
2. **Vue Test Utils**: For component mounting and interaction.

## 📏 Guidelines
1. **Unit Tests**: Test composables and stores in isolation.
2. **Component Tests**:
   - Verify rendering of props.
   - Test user interactions (clicks, inputs).
   - Ensure reactive state changes correctly.
3. **Mocking**: Use `vi.mock()` for API services and external dependencies.

## 🚀 Execution
Run tests using `pnpm test` or `pnpm vitest`.
