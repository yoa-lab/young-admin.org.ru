---
title: "Запуск Fail2ban в Debian 12 для SSH"
date: 2024-10-21
categories: 
  - "linux"
tags: 
  - "fail2ban"
---

Для работы fail2ban с логами journalctl вместо rsyslog

## Редактирование конфига

В конфиге fail2ban редактируем следующее:

```bash
#По умолчанию будет стоять auto, пример:
backend = auto
#Меняем с auto на systemd
backend = systemd
```

После замены сохраняем файл и перезапускаем демона:

```bash
service fail2ban restart
```

После перезапуска fail2ban перезапустится без ошибки отсутствия логов и всё заработает.

## Межсетевой экран

Я обычно использую iptables по старой памяти как его установить можно посмотреть [тут](https://young-admin.org.ru/ustanovka-i-nastrojka-fail2ban/#Установка_fail2ban_и_iptables).
