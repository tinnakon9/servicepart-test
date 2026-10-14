---
type: Reference
title: Java 8 (JDK/runtime)
description: >-
  ภาษาและ runtime ของโปรเจกต์: Java 1.8 ตามการตั้งค่า compiler ของ Eclipse
tags:
  - init-project
  - technology
sources:
  - resource: https://api.adoptium.net/v3/info/available_releases
    title: Adoptium API — available releases (LTS 25, Java 8 still available)
  - resource: https://docs.oracle.com/javase/8/docs/
    title: Java SE 8 documentation
  - resource: ../app/ServicePartCommon/.settings/org.eclipse.jdt.core.prefs
    title: Eclipse compiler settings of ServicePartCommon (compliance 1.8)
  - resource: ../app/ServicePartWeb/.settings/org.eclipse.jdt.core.prefs
    title: Eclipse compiler settings of ServicePartWeb (compliance 1.8)
generated:
  by: "claude-code/claude-sonnet-5-5"
  at: "2026-10-14T04:50:00Z"
status: stable
stale_after: 2026-11-13T04:50:00Z
verified:
  - by: "claude-code/claude-sonnet-5-5"
    at: "2026-10-14T04:50:00Z"
---

# Java 8 (JDK/runtime)

ตรวจสอบเมื่อ 2026-10-14

- **เวอร์ชันล่าสุด:** Adoptium ระบุ LTS ล่าสุดคือ Java 25 ส่วน Java 8 ยังมีให้ใช้ (build ล่าสุด `jdk8u504-b01`)
- **เวอร์ชันที่โปรเจกต์ใช้:** Java 1.8 — `org.eclipse.jdt.core.compiler.compliance=1.8` และ `source=1.8` ในไฟล์ `.settings` ของ ServicePartCommon และ ServicePartWeb
- โค้ดต้อง compile ที่ระดับ 1.8 จึงห้ามใช้ภาษาหรือ API ที่ใหม่กว่า Java 8
- driver ฐานข้อมูลที่ต้องเข้ากับ Java 8 ดู [microsoft-sql-server](microsoft-sql-server.md)

## ช่องว่างที่ยังไม่ได้ยืนยัน

- ไม่ทราบว่า runtime บนเซิร์ฟเวอร์ที่ deploy ใช้ JDK ตัวไหน
- CLI: ไม่มีเอกสารระบุว่าเขียน agent context file
