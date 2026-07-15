---
id: "article_320"
title: "Установка ИКС"
description: "Интернет-шлюз ИКС можно установить с диска, флеш-накопителя или использовать готовый образ виртуальной машины. Системные требования зависят от количества пользователей."
type: "article"
section: "ustanovka-iks"
parent_id: "category_9"
level: "2"
order: "7"
source_url: "https://doc.a-real.ru/index.php?article=320"
processed_at: "2026-07-14"
images_count: "0"
tags: "[икс, установка, firewall, системные_требования]"
---

Интернет-шлюз ИКС можно установить с различных носителей или использовать готовый образ виртуальной машины.

---

Интернет-шлюз ИКС можно установить с различных носителей или использовать готовый образ виртуальной машины:

- [с диска](ustanovka-iks-s-diska.md);
- [с флеш-накопителя](ustanovka-s-fleshki-2.md).

**Системные требования**

| Количество пользователей | Процессор | Жесткий диск | Оперативная память |
| --- | --- | --- | --- |
| 50—100 | Intel Core i3 12100F или аналогичный | 64 GB | 8 GB |
| 100—500 | Intel Core i5 12400F или аналогичный | 64—240 GB | 8—16 GB |
| более 500 | Intel Core i5-13400F или аналогичный | 480 GB | 16 GB и более |

> ⚠ Внимание! Убедитесь, что оборудование, на которое вы собираетесь устанавливать ИКС, соответствует системным требованиям FreeBSD. Мы гарантируем работу со [следующими серверами](https://xserver.a-real.ru/ics-hardware/). Проверить совместимость своего оборудования вы можете в [статье](https://www.freebsd.org/releases/14.3R/hardware/).

Системные требования в большей степени зависят от нагрузки на сервер, а именно — от количества используемых сервисов, таких как прокси, детектор атак, антивирус, а также от их настройки и активности пользователей.

Также ИКС доступен для установки на [виртуальную машину](ustanovka-iks-na-virtualnuyu-mashinu/ustanovka-iks-na-virtualnuyu-mashinu-obzor-2.md). Обеспечена поддержка следующих систем виртуализации:

- [VMware Workstation и VMware ESXi](ustanovka-iks-na-virtualnuyu-mashinu/ustanovka-iks-na-platformu-vmware-3.md)
- [VirtualBox](ustanovka-iks-na-virtualnuyu-mashinu/ustanovka-iks-na-virtualbox-2.md)
- [Hyper-V](ustanovka-iks-na-virtualnuyu-mashinu/ustanovka-iks-na-hyperv-2.md)
- [Proxmox Virtual Environment](ustanovka-iks-na-virtualnuyu-mashinu/ustanovka-iks-na-proxmox-virtual-environment-2.md)

Можно также воспользоваться [образом виртуальной машины](ustanovka-iks-na-virtualnuyu-mashinu/ustanovka-iks-na-virtualnuyu-mashinu-obzor-2.md) (virtual appliance).

> Видео: [https://vk.com/video_ext.php?oid=-18503994&id=456239321&hd=2](https://vk.com/video_ext.php?oid=-18503994&id=456239321&hd=2)
