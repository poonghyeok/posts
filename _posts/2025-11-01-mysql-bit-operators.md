---
title: Mysql Binary bit oprerators
author: poonghyeok
date: 2025-11-01
category: ["SQL","MYSQL"]
layout: post
mermaid: true
---

### 십진수를 이용해서 바로 2진수 비트연산
```sql
select (10 & 6) = 2; 
-- AND연산 ... 1010(2) & 110(2) => 10(2) = 2

select (10 | 6); 
-- OR연산 ... 14 ... 1010(2) | 110(2) => 1110(2) => 14

select (10 ^ 6); 
-- XOR연산 ... 12 ... 1010(2) | 110(2) => 1100(2) => 12
```
