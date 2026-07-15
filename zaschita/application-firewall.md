---
id: "article_73"
title: "Application Firewall"
description: "Модуль «Application Firewall» предназначен для отслеживания и блокирования трафика пользователей на основании категорий библиотеки nDPI, а также соединений пользователей через утилиту Xauth."
type: article
section: "zaschita"
parent_id: "category_20"
level: 2
order: 14
source_url: "https://doc.a-real.ru/index.php?article=73"
processed_at: "2026-07-15"
images_count: 5
tags: [икс, firewall, защита, фильтрация]
---

# Application Firewall

Модуль **«Application Firewall»** предназначен для отслеживания и блокирования трафика пользователей на основании категорий библиотеки nDPI, а также соединений пользователей, которые подключаются к ИКС через утилиту [Xauth](https://doc.a-real.ru/index.php?article=51).

Для открытия модуля перейдите в меню **Защита > Application Firewall**.

![Иллюстрация](../../../images/article_73/application_firewall.png)

В модуле расположены следующие вкладки:

- [Application Firewall](#tab1)
- [Настройки](#tab2)
- [Заблокированные соединения](#tab3)
- [Журнал](#tab4)

## Application Firewall

На данной вкладке отображается состояние службы «[Application Firewall](https://doc.a-real.ru/index.php?article=24/#application_firewall)»:

- статус службы (**запущен**, **остановлен**, **выключен**, **не настроен**);
- кнопка **«Включить»** (**«Выключить»**) — позволяет запустить или остановить службу;
- журнал последних событий.

![Иллюстрация](../../../images/article_73/application_firewall1.png)

## Настройки

Данная вкладка предназначена для настройки работы Application Firewall.

![Иллюстрация](../../../images/article_73/application_firewall2.png)

На вкладке можно выбрать **доступные сети**, в которых будет производиться сканирование соединений пользователей. По умолчанию установлены локальные сети.

Чтобы изменения вступили в силу, нажмите **«Сохранить»**.

## Заблокированные соединения

На данной вкладке отображается список заблокированных соединений тех пользователей, которым назначены [запрещающие правила Application Firewall](https://doc.a-real.ru/index.php?article=148) или у которых заблокированы процессы Xauth.

![Иллюстрация](../../../images/article_73/application_firewall3.png)

## Журнал

На данной вкладке отображается сводка всех системных сообщений модуля с указанием даты и времени.

![Иллюстрация](../../../images/article_73/application_firewall4.png)

[Журнал](https://doc.a-real.ru/index.php?article=196#summary) является стандартным элементом веб-интерфейса ИКС.

> ⚠ Внимание! Кнопка **«Удалить логи»** удаляет все логи, которые ведутся модулем **«Application Firewall»**.

---

**Источник:** [Документация ИКС — Application Firewall](https://doc.a-real.ru/index.php?article=73)
