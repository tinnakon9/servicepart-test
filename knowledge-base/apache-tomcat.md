---
type: Reference
title: Apache Tomcat
description: >-
  servlet container ที่ใช้รันเว็บและ job ของโปรเจกต์ (เวอร์ชันที่ใช้จริงยังไม่ทราบ)
tags:
  - init-project
  - technology
sources:
  - resource: https://tomcat.apache.org/whichversion.html
    title: Apache Tomcat — Which version do I want
  - resource: https://tomcat.apache.org/tomcat-9.0-doc/index.html
    title: Apache Tomcat 9.0 documentation
  - resource: https://repo1.maven.org/maven2/org/apache/tomcat/tomcat/maven-metadata.xml
    title: Maven Central metadata — tomcat (9.0.123 ล่าสุดของสาย 9)
  - resource: ../app/ServicePartLib/tomcatJobLib
    title: โฟลเดอร์ jar สำหรับ job ที่รันบน Tomcat
generated:
  by: "claude-code/claude-sonnet-5-5"
  at: "2026-10-14T04:50:00Z"
status: stable
stale_after: 2026-11-13T04:50:00Z
verified:
  - by: "claude-code/claude-sonnet-5-5"
    at: "2026-10-14T04:50:00Z"
---

# Apache Tomcat

ตรวจสอบเมื่อ 2026-10-14

- **เวอร์ชันล่าสุด:** สาย 11.0.x (stable, Servlet 6.1) และ 10.1.x; สาย 9.x ล่าสุดคือ 9.0.123
- **เวอร์ชันที่โปรเจกต์ใช้:** ไม่ทราบ (ดูช่องว่างด้านล่าง)
- **บทบาท:** servlet container รัน ServicePartWeb และ ServicePartJob; มีโฟลเดอร์ `app/ServicePartLib/tomcatJobLib` สำหรับ jar ของ job
- หน้า whichversion ระบุว่า Tomcat 10.1.x implement Servlet 6.0 และ 11.0.x implement Servlet 6.1 ยังไม่ได้ตรวจความเข้ากันได้กับ Struts 2.2.1 จึงอย่าเปลี่ยนสาย Tomcat โดยไม่ตรวจก่อน

## ช่องว่างที่ยังไม่ได้ยืนยัน

- ไม่ทราบเวอร์ชัน Tomcat ที่ใช้ใน production หรือเครื่อง dev
- CLI: ไม่มีเอกสารระบุว่าเขียน agent context file
