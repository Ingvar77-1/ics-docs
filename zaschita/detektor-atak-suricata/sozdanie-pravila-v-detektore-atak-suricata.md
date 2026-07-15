---
id: "article_424"
title: "Создание правила в Детекторе атак Suricata"
description: "Создание правила в Детекторе атак Suricata на примере исключения для IP-адреса."
type: "article"
section: "zaschita/detektor-atak-suricata"
parent_id: "category_101"
level: "3"
order: "3"
source_url: "https://doc.a-real.ru/index.php?article=424"
processed_at: "2026-07-14"
images_count: "0"
tags: "[икс, детектор атак, suricata, firewall, настройка]"
---

Создание правила в Детекторе атак Suricata на примере исключения для IP-адреса.

---

В данной статье рассматривается создание правила в Детекторе атак Suricata на примере исключения для IP-адреса.
Пример:
`pass ip 8.8.8.8 any <> $HOME_NET any (classtype:trojan-activity; sid:2008125;)`
либо:
`pass ip [8.8.8.0/24, 8.8.8.0/23] any -> $HOME_NET any (classtype:trojan-activity; sid:2008124;)`
Для создания правила выполните следующие действия:

1. Создайте **документ** формата txt.

2. Укажите **заголовок**. Это действие, которое необходимо сделать с трафиком. Возможные варианты: ALERT, DROP, PASS или REJECT.
Пример:
`pass ip 8.8.8.8 any <> $HOME_NET any (classtype:trojan-activity; sid:2008125;)`

3. Укажите необходимый **сетевой адрес**, для которого требуется сделать исключение. Это может быть IP-адрес либо интерфейс. Возможные интерфейсы: HOME_NET, EXTERNAL_NET и т.д. Соответственно, пропишите либо ip… , либо $..._NET.
Пример:
`pass ip 8.8.8.8 any <> $HOME_NET any (classtype:trojan-activity; sid:2008125;)`

4. В качестве **порта** можно указать any (то есть любой) либо прописать какой-то конкретный.
Пример:
`pass ip 8.8.8.8 any <> $HOME_NET 443 (classtype:trojan-activity; sid:2008125;)`

5. Укажите **направление трафика**:
- <> — будет работать для входящего и исходящего;
- -> — указывает, откуда и куда должен идти трафик.
Пример:
`pass ip 8.8.8.8 any <> $HOME_NET any (classtype:trojan-activity; sid:2008125;)`

6. Укажите **classtype**. Данный параметр определяет то, как будет классифицироваться (подписываться) сам трафик. 
Возможные варианты:
- attempted-admin — Attempted Administrator Privilege Gain
- attempted-user — Attempted User Privilege Gain
- inappropriate-content — Inappropriate Content was Detected
- policy-violation — Potential Corporate Privacy Violation
- shellcode-detect — Executable code was detected
- successful-admin — Successful Administrator Privilege Gain
- successful-user — Successful User Privilege Gain
- trojan-activity — A Network Trojan was detected
- unsuccessful-user — Unsuccessful User Privilege Gain
- web-application-attack — Web Application Attack
- attempted-dos — Attempted Denial of Service
- attempted-recon — Attempted Information Leak
- bad-unknown — Potentially Bad Traffic
- default-login-attempt — Attempt to login by a default username and password
- denial-of-service — Detection of a Denial of Service Attack
- misc-attack — Misc Attack
- non-standard-protocol — Detection of a non-standard protocol or event
- rpc-portmap-decode — Decode of an RPC Query
- successful-dos — Denial of Service
- successful-recon-largescale — Large Scale Information Leak
- successful-recon-limited — Information Leak
- suspicious-filename-detect — A suspicious filename was detected
- suspicious-login — An attempted login using a suspicious username was detected
- system-call-detect — A system call was detected
- unusual-client-port-connection — A client was using an unusual port
- web-application-activity — Access to a potentially vulnerable web application
- icmp-event — Generic ICMP event
- misc-activity — Misc activity
- network-scan — Detection of a Network Scan
- not-suspicious — Not Suspicious Traffic
- protocol-command-decode — Generic Protocol Command Decode
- string-detect — A suspicious string was detected
- unknown — Unknown Traffic
- tcp-connection — A TCP connection was detected very
Пример:
`pass ip 8.8.8.8 any <> $HOME_NET any (classtype:trojan-activity; sid:2008125;)`

7. Укажите значение sid (**номер идентификатора правила**). Рекомендуется использовать для локальных правил значение больше 1000000, так как значения от 0 до 999999 используются в правилах самого Snort.
Пример:
`pass ip 8.8.8.8 any <> $HOME_NET any (classtype:trojan-activity; sid:2008125;)`
