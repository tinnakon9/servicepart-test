---
type: Reference
title: โดเมน order และการค้นหา order no
description: >-
  การค้นหา order (firm order) และรายงานที่เกี่ยวข้อง
tags:
  - init-project
  - domain
sources:
  - resource: ../app/ServicePartWeb/src/struts-firmorder.xml
    title: struts-firmorder.xml
  - resource: ../app/ServicePartWeb/WebContent/jsp/firmorder
    title: JSP ของหน้า firm order
  - resource: ../app/ServicePartWeb/WebContent/jasper/ListFirmOrderReport.jrxml
    title: รายงาน list firm order
  - resource: the git history of this repository (commit messages), inspected 2026-10-14
generated:
  by: "claude-code/claude-sonnet-5-5"
  at: "2026-10-14T04:50:00Z"
status: stable
---

# โดเมน order และการค้นหา order no

## Scope

หน้าและรายงาน firm order รวมการค้นหาด้วย order no ไม่รวม forecast

## Current material

- `struts-firmorder.xml`, JSP ใน `WebContent/jsp/firmorder`, รายงาน `ListFirmOrderReport`
- commit "search order no" (0a9bfc4) และ "like to =" (46cf977) แก้เงื่อนไขการค้นหา
- ยังไม่มีเอกสาร business rule ของโดเมนนี้

## Open questions

- กติกาการค้นหา (exact หรือ like) ที่ถูกต้อง และคอลัมน์ที่ใช้ค้น ยังไม่ได้บันทึก
