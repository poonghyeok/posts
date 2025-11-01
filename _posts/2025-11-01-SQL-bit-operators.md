---
title: SQL Binary bit oprerators
author: poonghyeok
date: 2025-11-01
category: ["SQL","MYSQL"]
layout: post
mermaid: true
---

### 십진수를 이용해서 바로 2진수 비트연산
**MYSQL**
```sql
select (10 & 6) = 2; 
-- AND연산 ... 1010(2) & 110(2) => 10(2) = 2

select (10 | 6); 
-- OR연산 ... 14 ... 1010(2) | 110(2) => 1110(2) => 14

select (10 ^ 6); 
-- XOR연산 ... 12 ... 1010(2) | 110(2) => 1100(2) => 12
```
**ORACLE**
```sql
SELECT bitand(10, 6) FROM dual; 
-- AND연산 ... 2

SELECT 10 + 6 - bitand(10, 6) FROM dual;
-- OR연산 ... 14 ... BITOR는 따로 없고 위처럼 구현하나보다 => 그래서 XOR 연산은 별로 알고 싶지않다.
```