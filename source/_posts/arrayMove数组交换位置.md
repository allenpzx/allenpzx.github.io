---
title: 函数表现

tags:
  - JavaScript
categories:
  - JavaScript
---

```typescript
function arrayMove<T>(array: T[], oldIndex: number, newIndex: number): T[] {
  [array[oldIndex], array[newIndex]] = [array[newIndex], array[oldIndex]];
  return array;
}
```
