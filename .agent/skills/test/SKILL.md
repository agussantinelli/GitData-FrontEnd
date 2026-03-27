---
name: test
description: Guidelines for frontend component and E2E testing in GitData.
---

# 🧬 GitData Testing Overview

Universal rules for ensuring quality across the GitData Dashboards.

## 📏 Guidelines
1. **Unit & Integration**: Use Vitest + Vue Test Utils. Refer to `testing-strategy-fe` and `integration-testing`.
2. **E2E Testing**: Use Cypress for full-flow tests (User Search, Dashboard interaction).
3. **Mocking**: Use `vi.mock()` for services and Zod for generating mock data.
4. **Coverage**: Every business logic or UI component must have a `spec.ts` file.
