---
type: Reference
title: JasperReports
description: >-
  เครื่องมือสร้างรายงาน ใช้ jasperreports 4.0.0 ผ่านปลั๊กอิน Struts 2
tags:
  - init-project
  - technology
sources:
  - resource: https://repo1.maven.org/maven2/net/sf/jasperreports/jasperreports/maven-metadata.xml
    title: Maven Central metadata — jasperreports (release 7.0.8)
  - resource: ../app/ServicePartLib/lib/jasperreports-4.0.0.jar
    title: jasperreports-4.0.0.jar ที่โปรเจกต์ใช้
  - resource: ../app/ServicePartLib/lib/struts2-jasperreports-plugin-2.2.1.jar
    title: ปลั๊กอิน Struts 2 สำหรับ JasperReports
  - resource: ../app/ServicePartWeb/WebContent/jasper/ListFirmOrderReport.jrxml
    title: ตัวอย่างเทมเพลตรายงาน (.jrxml)
generated:
  by: "claude-code/claude-sonnet-5-5"
  at: "2026-10-14T04:50:00Z"
status: stable
stale_after: 2026-11-13T04:50:00Z
verified:
  - by: "claude-code/claude-sonnet-5-5"
    at: "2026-10-14T04:50:00Z"
---

# JasperReports

ตรวจสอบเมื่อ 2026-10-14

- **เวอร์ชันล่าสุด:** 7.0.8 (Maven Central, อัปเดต 2026-08-05)
- **เวอร์ชันที่โปรเจกต์ใช้:** 4.0.0 (`jasperreports-4.0.0.jar`) พร้อม `jasperreports-chart-themes-4.0.0.jar`, `jasperreports-fonts-4.0.0.jar`
- **ตำแหน่งเทมเพลต:** `app/ServicePartWeb/WebContent/jasper/` มีทั้ง `.jrxml` (ต้นฉบับ) และ `.jasper` (compile แล้ว) เช่น `ListFirmOrderReport` และ `ForecastReport`
- **การเชื่อมกับ Struts:** `struts2-jasperreports-plugin-2.2.1.jar` ดู [struts2](struts2.md)

## ช่องว่างที่ยังไม่ได้ยืนยัน

- ลิงก์เอกสารทางการของ Jaspersoft ตอบ HTTP 403 ตอนตรวจ จึงยังไม่มี docs URL ในเอกสารนี้
- CLI: ไม่มีเอกสารระบุว่าเขียน agent context file
