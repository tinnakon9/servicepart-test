---
type: Reference
title: Microsoft SQL Server (JDBC)
description: >-
  ฐานข้อมูลของโปรเจกต์ เข้าถึงผ่าน Microsoft JDBC driver (sqljdbc4.jar) และ Hibernate
tags:
  - init-project
  - technology
sources:
  - resource: https://repo1.maven.org/maven2/com/microsoft/sqlserver/mssql-jdbc/maven-metadata.xml
    title: Maven Central metadata — mssql-jdbc (13.6.0.jre11 ล่าสุด)
  - resource: https://learn.microsoft.com/en-us/sql/connect/jdbc/microsoft-jdbc-driver-for-sql-server
    title: Microsoft JDBC Driver for SQL Server
  - resource: ../app/ServicePartLib/lib/sqljdbc4.jar
    title: sqljdbc4.jar ที่โปรเจกต์ใช้
  - resource: ../app/ServicePartModel/hibernate.properties
    title: hibernate.properties (dialect และ URL ไม่คัดลอกค่าการเชื่อมต่อ)
generated:
  by: "claude-code/claude-sonnet-5-5"
  at: "2026-10-14T04:50:00Z"
status: stable
stale_after: 2026-11-13T04:50:00Z
verified:
  - by: "claude-code/claude-sonnet-5-5"
    at: "2026-10-14T04:50:00Z"
---

# Microsoft SQL Server (JDBC)

ตรวจสอบเมื่อ 2026-10-14

- **เวอร์ชัน driver ล่าสุด:** `mssql-jdbc` 13.6.0.jre11 (Maven Central, อัปเดต 2026-09-10) — build นี้ติดป้าย jre11 ซึ่งสูงกว่า Java 8 ที่โปรเจกต์ใช้
- **driver ที่โปรเจกต์ใช้:** `sqljdbc4.jar` และ `sqljdbc.jar` ใน `app/ServicePartLib/lib` (และ `sqljdbc4.jar` ใน `tomcatJobLib`)
- **การเชื่อมต่อ:** กำหนดผ่าน Hibernate ใน `app/ServicePartModel/hibernate.properties` และ `src/hibernate.cfg.xml` โดยใช้ `SQLServerDialect` ห้ามคัดลอกค่าการเชื่อมต่อลงเอกสาร

## ช่องว่างที่ยังไม่ได้ยืนยัน

- ไม่ทราบเวอร์ชันของ SQL Server server ที่ใช้จริง
- ยังไม่ได้ตรวจว่ามี driver build ที่รองรับ Java 8 สำหรับ 13.x หรือไม่ (ค่า metadata ที่เห็นเป็น jre11)
- CLI: ไม่มีเอกสารระบุว่าเขียน agent context file
