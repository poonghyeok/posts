---
title: Mysql functions
author: poonghyeok
date: 2025-11-01
category: ["SQL","MYSQL"]
layout: post
mermaid: true
---

### 진수 변환 사용하기
```sql
select conv(7, 10, 2); -- 10진수 7을 2진수로 변환
--- 111

select conv(111, 2, 10); -- 2진수 111을 10진수로 변환
--- 7
```

### num <-> string conver
```sql
select cast(123 as char(10)); --- '123'
select convert(123, char); --- '123'
select concat(123, '') --- ''

select cast('123', as unsigned) --- 123
select convert('123', unsigned) --- 123
select convert('-123', signed) --- -123
--- 음수처리하기 위해서 signed 사용
```