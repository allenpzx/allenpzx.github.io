---
title: 函数表现
date: {{ date }}
tags:
- JavaScript
---


```typescript
function arrayMove<T>(array: T[], oldIndex: number, newIndex: number): T[] {
  [array[oldIndex], array[newIndex]] = [array[newIndex], array[oldIndex]];
  return array;
}
```