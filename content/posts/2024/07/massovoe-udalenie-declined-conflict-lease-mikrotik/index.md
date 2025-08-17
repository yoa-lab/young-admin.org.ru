---
title: "Массовое удаление Declined, Conflict lease Mikrotik"
date: 2024-07-26
categories: 
  - "mikrotik"
  - "setevoe-oborudovanie"
tags: 
  - "komandy"
---

На mikrtoik массово завиcли клиенты в статусе conflict и declined. У меня lease-time несколько суток, чтобы ошибочные долго не весели, решил удалить их сразу после исправления ошибки из-за которой они появились.

Команда для терминала mikrotik'а, чтобы массово удалить:

```
/ip dhcp-server lease remove [find status=declined]
/ip dhcp-server lease remove [find status=conflict]
```
