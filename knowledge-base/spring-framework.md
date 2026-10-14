---
type: Reference
title: Spring Framework
description: >-
  Spring 2.5 อยู่ใน classpath แต่โค้ดของโปรเจกต์แทบไม่เรียกใช้โดยตรง
tags:
  - init-project
  - technology
sources:
  - resource: https://github.com/spring-projects/spring-framework/releases
    title: Spring Framework releases (v7.0.9 latest)
  - resource: https://docs.spring.io/spring-framework/reference/
    title: Spring Framework reference
  - resource: ../app/ServicePartLib/lib/spring.jar
    title: spring.jar (Spring-Version 2.5 ใน MANIFEST)
  - resource: ../app/ServicePartWeb/src/log4j.xml
    title: log4j.xml — ที่เดียวที่อ้างถึง org.springframework ใน source ของ ServicePartWeb
generated:
  by: "claude-code/claude-sonnet-5-5"
  at: "2026-10-14T04:50:00Z"
status: stable
stale_after: 2026-11-13T04:50:00Z
verified:
  - by: "claude-code/claude-sonnet-5-5"
    at: "2026-10-14T04:50:00Z"
---

# Spring Framework

ตรวจสอบเมื่อ 2026-10-14

- **เวอร์ชันล่าสุด:** 7.0.9 (release เมื่อ 2026-08-20)
- **เวอร์ชันที่โปรเจกต์ใช้:** 2.5 (`spring.jar` รวมโมดูลไว้ใน jar เดียวใน `app/ServicePartLib/lib`)
- **บทบาท:** library ช่วยเสริม ไม่ใช่กรอบหลักของแอป
- จากการค้น `org.springframework` ใน `ServicePart*/src`, `MergeFile/src` และ `web.xml` พบเพียง `app/ServicePartWeb/src/log4j.xml` จึงไม่มี Spring listener ใน `web.xml` และไม่พบ import ของ Spring ใน source ตอนตรวจ
- Hibernate ของโปรเจกต์ไม่ได้ผ่าน Spring ORM ดู [hibernate](hibernate.md)

## ช่องว่างที่ยังไม่ได้ยืนยัน

- ยังไม่ทราบว่ามีโค้ดส่วนใดโหลด Spring ผ่านทางอื่น (เช่น reflection หรือไฟล์ config นอก source)
- CLI: ไม่มีเอกสารระบุว่าเขียน agent context file
