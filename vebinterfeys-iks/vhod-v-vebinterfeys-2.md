---
id: "article_21"
title: "Вход в веб-интерфейс"
description: "Описание процесса входа в веб-интерфейс управления ИКС: ввод IP-адреса и порта, ввод логина root и пароля 00000, рекомендации по безопасности."
type: "article"
section: "vebinterfeys-iks"
parent_id: "category_16"
level: "2"
order: "2"
source_url: "https://doc.a-real.ru/index.php?article=21"
processed_at: "2026-07-13"
images_count: "1"
tags: "[икс, веб-интерфейс, авторизация, вход, администрирование]"
---

После установки можно приступить к работе в веб-интерфейсе ИКС.

---

Чтобы войти в веб-интерфейс управления ИКС на любом компьютере из локальной сети, в браузере введите [IP-адрес](../o-dokumentacii/slovar-terminov-3.md) сервера, который был указан при установке, и порт 81 (&lt;ip:81&gt;).

&gt; ⚠ Внимание! В качестве браузера по умолчанию рекомендуется использовать Mozilla Firefox или Google Chrome.

На экране начнется процесс загрузки веб-интерфейса и появится окно ввода **логина** и **пароля**.

![Вход в веб-интерфейс ИКС](../images/article_21/start-12.3.png)

При первом входе в веб-интерфейс необходимо использовать логин **root** и пароль **00000** (пять нулей).

&gt; ⚠ Внимание! Настоятельно рекомендуется поменять пароль администратора сразу же после первого входа в систему. В противном случае к интерфейсу управления ИКС смогут получить доступ посторонние лица.

В окне авторизации расположены ссылки:

- [Xauth](../polzovateli-i-statistika/server-avtorizacii-xauth/server-avtorizacii-xauth-obzor-2.md) (с возможностью выбрать, какой Xauth скачать);
- [Captive Portal](../polzovateli-i-statistika/captive-portal/captive-portal-obzor-2.md);
- [Веб-почта](../pochta/vebpochta/vebpochta-obzor-2.md);
- [Xphone](https://doc.a-real.ru/index.php?article=101).

При успешной [авторизации](../o-dokumentacii/slovar-terminov-3.md) на экране появится [главная страница ИКС](https://doc.a-real.ru/index.php?article=22).

После первого входа в веб-интерфейс необходимо провести [первичную настройку системы](master-nachalnoy-nastroyki-sistemy-2.md).
