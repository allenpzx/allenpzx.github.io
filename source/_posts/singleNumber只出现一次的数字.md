---
title: singleNumber
date: {{ date }}
tags:
- JavaScript
categories:
- JavaScript
---

```typescript
/**
 * @param {number[]} nums
 * @return {number}
 */
var singleNumber = function(nums: number[]) {
    return [...nums.reduce((prev, v)=>{
        prev.has(v) ? prev.delete(v) : prev.add(v);
        return prev
    }, new Set())][0];
};
```