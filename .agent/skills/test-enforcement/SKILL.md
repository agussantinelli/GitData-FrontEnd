---
name: test-enforcement
description: Mandatory rule requiring a corresponding test file for every business logic file and UI component in GitData.
---

# 🚔 GitData Test Enforcement

To ensure reliability, every file must have a corresponding test file.

## 📏 Rules
1. **Rule of One**: Every `.ts` or `.vue` file in `src/services`, `src/stores`, `src/composables`, or `src/components` MUST have a matching `.spec.ts` or `.test.ts` file.
2. **Location**: Test files must be located in the same directory as the file they are testing.
3. **Naming**: `[filename].spec.ts`.
4. **Tools**: Use Vitest and Vue Test Utils (@vue/test-utils).
5. **Simultaneous Creation**: If a file is created, its test MUST be created in the same step.
