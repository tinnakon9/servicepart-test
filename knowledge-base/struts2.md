---
type: Reference
title: Apache Struts 2
description: >-
  web MVC framework ของ ServicePartWeb ใช้ Struts 2.2.1
tags:
  - init-project
  - technology
sources:
  - resource: https://struts.apache.org/download.cgi
    title: Apache Struts downloads (7.4.0 best available, 6.12.0)
  - resource: https://struts.apache.org/getting-started/
    title: Apache Struts getting started
  - resource: ../app/ServicePartLib/lib/struts2-core-2.2.1.jar
    title: struts2-core-2.2.1.jar ที่โปรเจกต์ใช้
  - resource: ../app/ServicePartWeb/WebContent/WEB-INF/web.xml
    title: web.xml ที่ลงทะเบียน StrutsPrepareAndExecuteFilter
  - resource: ../app/ServicePartWeb/src/struts.xml
    title: struts.xml ของ ServicePartWeb
generated:
  by: "claude-code/claude-sonnet-5-5"
  at: "2026-10-14T04:50:00Z"
status: stable
stale_after: 2026-11-13T04:50:00Z
verified:
  - by: "claude-code/claude-sonnet-5-5"
    at: "2026-10-14T04:50:00Z"
---

# Apache Struts 2

ตรวจสอบเมื่อ 2026-10-14

- **เวอร์ชันล่าสุด:** 7.4.0 (best available) และ 6.12.0 — หน้า download แนะนำให้ย้ายไปรุ่นล่าสุดเมื่อทำได้
- **เวอร์ชันที่โปรเจกต์ใช้:** 2.2.1 (`struts2-core-2.2.1.jar` ใน `app/ServicePartLib/lib`) ซึ่งเก่ากว่ารุ่นล่าสุดมาก
- **บทบาท:** web MVC ของ ServicePartWeb — `web.xml` ลงทะเบียนฟิลเตอร์ `org.apache.struts2.dispatcher.ng.filter.StrutsPrepareAndExecuteFilter`
- **การตั้งค่า:** แยกไฟล์ตามฟีเจอร์เป็น `struts-*.xml` ใน `app/ServicePartWeb/src` (เช่น `struts-asn.xml`, `struts-firmorder.xml`) โดยมี `struts.xml` เป็นไฟล์หลัก
- รายงาน Jasper ผ่านปลั๊กอิน `struts2-jasperreports-plugin-2.2.1.jar` ดู [jasperreports](jasperreports.md)

## ช่องว่างที่ยังไม่ได้ยืนยัน

- ยังไม่ได้ตรวจแผนย้ายไป Struts รุ่นใหม่ และความเข้ากันได้กับ Java 8
- CLI: ไม่มีเอกสารระบุว่าเขียน agent context file
