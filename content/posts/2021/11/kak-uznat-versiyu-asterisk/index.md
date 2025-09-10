---
title: "Как узнать версию Asterisk"
date: 2021-11-03
categories: 
  - "asterisk"
tags: 
  - "komandy-terminala"
description: "Как определить версию Asterisk: способы проверки версии через CLI и команды Linux"
---

Версию можно узнать набрав в терминале:

```bash
# rasterisk
# core show version
```

Либо:

```bash
# asterisk -rx "core show version"
```

Или через терминал, без ипользования консоли Asterisk. Обратите внимание что команда с заглавной буквой V, если не работает то можно попробовать со строчной v:

```bash
# asterisk -V
```
