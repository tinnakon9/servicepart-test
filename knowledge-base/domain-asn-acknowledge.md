---
type: Reference
title: โดเมน ASN และ acknowledge
description: >-
  การรับ ASN และการยืนยันรับ (acknowledge) ของอะไหล่
tags:
  - init-project
  - domain
sources:
  - resource: ../app/ServicePartWeb/src/struts-asn.xml
    title: struts-asn.xml
  - resource: ../app/ServicePartWeb/WebContent/jasper/deliveryTagReport.jrxml
    title: เทมเพลตรายงาน delivery tag
  - resource: ../app/ServicePartWeb/WebContent/jsp/asn
    title: JSP ของหน้า ASN
  - resource: the git history of this repository (commit messages), inspected 2026-10-14
generated:
  by: "claude-code/claude-sonnet-5-5"
  at: "2026-10-14T04:50:00Z"
status: stable
---

# โดเมน ASN และ acknowledge

## Scope

หน้าและตรรกะที่เกี่ยวกับ ASN และการ acknowledge ใน ServicePartWeb ไม่รวมรายงาน delivery tag (ดู [domain-delivery-tag-report](domain-delivery-tag-report.md))

## Current material

- `struts-asn.xml`, `struts-acknowledge.xml`, `struts-adminacknowledge.xml` ใน `app/ServicePartWeb/src` และ JSP ใน `WebContent/jsp/asn`
- ประวัติ git มี commit "fixed check error data from Asn" (43452d3) ซึ่งแก้การตรวจข้อมูลผิดพลาดของ ASN
- ยังไม่มีเอกสาร business rule ของโดเมนนี้

## Open questions

- กฎการตรวจข้อมูล ASN และสถานะของ acknowledge ยังไม่ได้บันทึก
