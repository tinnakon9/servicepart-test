---
type: Reference
title: Hibernate ORM
description: >-
  ORM ของโปรเจกต์ในโมดูล ServicePartModel ใช้ Hibernate 3.3.2.GA
tags:
  - init-project
  - technology
sources:
  - resource: https://hibernate.org/orm/releases/
    title: Hibernate ORM releases (7.4.13.Final latest stable)
  - resource: https://hibernate.org/orm/documentation/
    title: Hibernate ORM documentation
  - resource: ../app/ServicePartLib/lib/hibernate-core-3.3.2.GA.jar
    title: hibernate-core-3.3.2.GA.jar ที่โปรเจกต์ใช้
  - resource: ../app/ServicePartModel/src/hibernate.cfg.xml
    title: hibernate.cfg.xml ของ ServicePartModel
  - resource: ../app/ServicePartModel/src/hibernate-partreceive.reveng.xml
    title: hibernate-partreceive.reveng.xml (reverse engineering config)
  - resource: ../app/ServicePartModel/hibernate.properties
    title: hibernate.properties (มีค่าการเชื่อมต่อ ไม่คัดลอกมาที่นี่)
generated:
  by: "claude-code/claude-sonnet-5-5"
  at: "2026-10-14T04:50:00Z"
status: stable
stale_after: 2026-11-13T04:50:00Z
verified:
  - by: "claude-code/claude-sonnet-5-5"
    at: "2026-10-14T04:50:00Z"
---

# Hibernate ORM

ตรวจสอบเมื่อ 2026-10-14

- **เวอร์ชันล่าสุด:** ORM 7.4.13.Final (stable) — ยังมีสาย 7.3, 7.2, 7.1 และ 6.6
- **เวอร์ชันที่โปรเจกต์ใช้:** 3.3.2.GA (`hibernate-core-3.3.2.GA.jar`, `hibernate3.jar`, `hibernate-annotations.jar`, `hibernate-entitymanager-3.4.0.GA.jar`)
- **บทบาท:** ORM ของโมดูล `ServicePartModel` (entity และ DAO)
- **การตั้งค่า:** `app/ServicePartModel/src/hibernate.cfg.xml`, `hibernate.properties`, และ `hibernate-partreceive.reveng.xml` สำหรับ reverse engineering จากฐานข้อมูล
- **Dialect:** `org.hibernate.dialect.SQLServerDialect` ดู [microsoft-sql-server](microsoft-sql-server.md)
- ค่าการเชื่อมต่อฐานข้อมูลอยู่ในไฟล์ที่อ้างด้านบน ห้ามคัดลอกค่าเหล่านั้นลงเอกสาร

## ช่องว่างที่ยังไม่ได้ยืนยัน

- CLI: ไม่มีเอกสารระบุว่าเขียน agent context file
