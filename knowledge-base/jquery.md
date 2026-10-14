---
type: Reference
title: jQuery
description: >-
  ไลบรารี JavaScript ฝั่ง client ใช้ jQuery 3.7.1 ใน ServicePartWeb
tags:
  - init-project
  - technology
sources:
  - resource: https://github.com/jquery/jquery/releases
    title: jQuery releases (4.0.0 latest)
  - resource: https://api.jquery.com/
    title: jQuery API documentation
  - resource: ../app/ServicePartWeb/WebContent/js/jquery3.7.1.min.js
    title: jquery3.7.1.min.js ที่โปรเจกต์ใช้
generated:
  by: "claude-code/claude-sonnet-5-5"
  at: "2026-10-14T04:50:00Z"
status: stable
stale_after: 2026-11-13T04:50:00Z
verified:
  - by: "claude-code/claude-sonnet-5-5"
    at: "2026-10-14T04:50:00Z"
---

# jQuery

ตรวจสอบเมื่อ 2026-10-14

- **เวอร์ชันล่าสุด:** 4.0.0 (release เมื่อ 2026-01-18)
- **เวอร์ชันที่โปรเจกต์ใช้:** 3.7.1 (`app/ServicePartWeb/WebContent/js/jquery3.7.1.min.js`)
- **สคริปต์ของโปรเจกต์:** `util.js` และ `public.js` ในโฟลเดอร์ `js` เดียวกัน
- ไม่มี SPA framework หรือ bundler; หน้าเป็น JSP และสคริปต์ถูกโหลดตรงจาก `WebContent/js`

## ช่องว่างที่ยังไม่ได้ยืนยัน

- ยังไม่ได้ตรวจว่าแต่ละ JSP โหลด jQuery ไฟล์ไหน และมีปลั๊กอินเสริมหรือไม่
- CLI: ไม่มีเอกสารระบุว่าเขียน agent context file
