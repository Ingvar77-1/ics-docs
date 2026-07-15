---
id: "article_231"
title: "Примеры почтовых фильтров"
description: "Примеры использования почтовых фильтров ИКС с регулярными выражениями для фильтрации входящих и исходящих сообщений."
type: "article"
section: "pochta/filtry"
parent_id: "category_48"
level: "3"
order: "3"
source_url: "https://doc.a-real.ru/index.php?article=231"
processed_at: "2026-07-15"
images_count: "0"
tags: "[икс, почта, фильтры, регулярные выражения, smtp]"
---

## Почтовые фильтры поддерживают следующие регулярные выражения:

```
%s = sender
%r = recipient
%Y(M) = date
%u = recipient user
%d = recipient domain
%Su = sender user
%Sd = sender domain
```

## Переместить исходящие в папку для IMAP-подключений

Условие: Отправитель содержит @domain

Действие: Отправить копию на %Su@domain/Sent

## Скопировать сообщения для пользователей в ящики другого домена

Условие: Получатель содержит @domain

Действие: Отправить копию на %u@domain2

## Если сообщение пришло от @domain2, положить его в спам

Условие: Отправитель содержит @domain2

Действие: Переместить в %Su@domain/Junk
