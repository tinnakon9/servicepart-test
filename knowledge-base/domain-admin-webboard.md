---
type: Reference
title: โดเมน admin และ webboard
description: >-
  ส่วนผู้ดูแลระบบและกระดานข่าว (webboard) ของ ServicePartWeb
tags:
  - init-project
  - domain
sources:
  - resource: ../app/ServicePartWeb/src/struts-adminwebboard.xml
    title: struts-adminwebboard.xml
  - resource: ../app/ServicePartWeb/src/struts-webboard.xml
    title: struts-webboard.xml
  - resource: ../app/ServicePartWeb/src/struts-adminacknowledge.xml
    title: struts-adminacknowledge.xml
generated:
  by: "claude-code/claude-sonnet-5-5"
  at: "2026-10-14T04:50:00Z"
status: stable
---

# โดเมน admin และ webboard

## Scope

ฟังก์ชันของผู้ดูแลระบบ (`adminIndex.jsp`, `indexAdmin.jsp`, `adminLogin.jsp`) และ webboard

## Current material

- `struts-adminwebboard.xml`, `struts-webboard.xml`, `struts-adminacknowledge.xml` ใน `app/ServicePartWeb/src`
- ยังไม่มีเอกสาร business rule ของโดเมนนี้

## Open questions

- สิทธิ์ของแต่ละบทบาท (admin/ผู้ใช้ทั่วไป) ยังไม่ได้บันทึก
