---
type: Reference
title: โดเมน delivery tag report
description: >-
  รายงาน delivery tag ที่ถูกแก้ไขบ่อยในประวัติ commit ล่าสุด
tags:
  - init-project
  - domain
sources:
  - resource: ../app/ServicePartWeb/WebContent/jasper/deliveryTagReport.jrxml
    title: เทมเพลตรายงาน delivery tag
  - resource: ../app/ServicePartWeb/src/struts-asn.xml
    title: struts-asn.xml
  - resource: the git history of this repository (commit messages), inspected 2026-10-14
generated:
  by: "claude-code/claude-sonnet-5-5"
  at: "2026-10-14T04:50:00Z"
status: stable
---

# โดเมน delivery tag report

## Scope

รายงาน delivery tag (Jasper) และข้อมูลที่ป้อนให้รายงาน ไม่รวมการรับ ASN

## Current material

- เทมเพลต `deliveryTagReport.jrxml` ใน `app/ServicePartWeb/WebContent/jasper`
- commit ล่าสุดหลายรายการแก้รายงานนี้ ("change delivery tag report", "update report delivery", "fix delivery tag report") และ "deli qty not fully displaying"
- เทคโนโลยีที่เกี่ยวข้อง: [jasperreports](jasperreports.md)

## Open questions

- รูปแบบ tag ที่ผู้ใช้ต้องการและความสัมพันธ์กับ ASN ยังไม่ได้บันทึก
