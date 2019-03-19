---
title: Использование Microsoft Graph Security API
description: Microsoft Graph Security API обеспечивает единый интерфейс и схему интеграции с решениями безопасности от корпорации Майкрософт и партнеров экосистемы. Это позволяет клиентам упростить операции, связанные с безопасностью, и лучше защититься от возрастающих киберугроз. Microsoft Graph Security API можно использовать в качестве службы агрегирования федеративных данных о безопасности, чтобы отправлять запросы всем подключенным поставщикам безопасности для получения агрегированных откликов. Используйте Microsoft Graph Security API для создания приложений с указанными ниже возможностями.
localization_priority: Priority
author: preetikr
ms.prod: security
ms.openlocfilehash: bd208067c2194766bb5f3d93d0caa21be086dca0
ms.sourcegitcommit: cd4bdb2c6754b1d5658e68909ea6c219466da6df
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/16/2019
ms.locfileid: "30644267"
---
# <a name="use-the-microsoft-graph-security-api"></a>Использование Microsoft Graph Security API

Microsoft Graph Security API обеспечивает единый интерфейс и схему интеграции с решениями безопасности от корпорации Майкрософт и партнеров экосистемы. Это позволяет клиентам упростить операции, связанные с безопасностью, и лучше защититься от возрастающих киберугроз. Microsoft Graph Security API объединяет запросы для всех подключенных поставщиков безопасности и собирает ответы. Используйте Microsoft Graph Security API для создания приложений с указанными ниже возможностями.

- объединение и корреляция оповещений системы безопасности из нескольких источников;
- разблокировка контекстных данных для получения сведений при расследованиях;
- автоматизация задач безопасности, бизнес-процессов, рабочих процессов и создания отчетов;
- отправка индикаторов угроз в продукты Майкрософт для настроенных обнаружений;
- вызов действий в ответ на новые угрозы;
- обеспечение видимости данных безопасности, чтобы использовать профилактическое управление рисками.

Microsoft Graph Security API включает указанные ниже ключевые объекты.

## <a name="alerts"></a>Оповещения

Оповещения — это потенциальные проблемы безопасности в клиенте пользователя, выявленные решениями по обеспечению безопасности корпорации Майкрософт или партнеров и помеченные для действия или уведомления. С помощью объекта [alerts](alert.md) Microsoft Graph Security можно объединить и оптимизировать управление проблемами безопасности во всех интегрированных решениях. Это также позволит приложениям коррелировать оповещения и контекст для улучшения защиты от угроз и отклика на них. Благодаря функции обновления оповещений можно синхронизировать состояние определенных оповещений в разных продуктах и службах обеспечения безопасности, интегрированных с Microsoft Graph Security API, с помощью обновления объекта [alerts](alert.md).

При использовании Microsoft Graph Security API доступны оповещения от указанных ниже поставщиков. Поддержка оповещений GET, PATCH (обновления доступны при использовании Microsoft Graph Security API, но могут быть недоступны в интерфейсе управления поставщика) и подписки (с помощью веб-перехватчиков) представлена в таблице ниже.

| Поставщик безопасности | <p align="center">Оповещение GET</p>| <p align="center">Оповещение PATCH</p>| <p align="center">Подписка на оповещения</p>|
|:------------------|:---------|:-----------|:------------------|
|[Центр безопасности Azure](https://docs.microsoft.com/azure/security-center/security-center-alerts-type)| <p align="center">&#x2713;</p> | <p align="center">&#x2713;</p> | <p align="center">&#x2713;</p> |
|[Защита идентификации Azure Active Directory](https://docs.microsoft.com/azure/active-directory/identity-protection/playbook) | <p align="center">&#x2713;</p> | <p align="center">&#x2713;</p> | <p align="center">&#x2713;</p> |
| [Microsoft Cloud App Security](https://docs.microsoft.com/cloud-app-security/monitor-alerts) | <p align="center">&#x2713;</p> | <p align="center">&#x2713;</p> | <p align="center">&#x2713;</p> |
|[Advanced Threat Protection в Защитнике Windows](https://docs.microsoft.com/windows/security/threat-protection/windows-defender-atp/attack-simulations-windows-defender-advanced-threat-protection)| <p align="center">&#x2713;</p> | <p align="center">&#x2713;</p> | <p align="center"> [Уведомление о проблеме](https://github.com/microsoftgraph/security-api-solutions/issues/new) </p> |
|[Расширенная защита от угроз Azure](https://docs.microsoft.com/azure-advanced-threat-protection/understanding-security-alerts#security-alert-categories)| <p align="center">&#x2713;</p> | <p align="center"> [Уведомление о проблеме](https://github.com/microsoftgraph/security-api-solutions/issues/new) </p> | <p align="center"> [Уведомление о проблеме](https://github.com/microsoftgraph/security-api-solutions/issues/new) </p> |
|Office 365 <ul><li> [По умолчанию](https://docs.microsoft.com/ru-RU/office365/securitycompliance/alert-policies#default-alert-policies)</li> <li>[Cloud App Security](https://docs.microsoft.com/ru-RU/office365/securitycompliance/anomaly-detection-policies-in-ocas)</li></ul> | <p align="center">&#x2713;</p> | <p align="center"> [Уведомление о проблеме](https://github.com/microsoftgraph/security-api-solutions/issues/new) </p> | <p align="center"> [Уведомление о проблеме](https://github.com/microsoftgraph/security-api-solutions/issues/new) </p> |
|[Azure Information Protection](https://docs.microsoft.com/azure/information-protection/faqs#i-see-azure-information-protection-is-listed-as-a-security-provider-for-microsoft-graph-securityhow-does-this-work-and-what-alerts-will-i-receive) **(предварительная версия)**| <p align="center">&#x2713;</p> | <p align="center">&#x2713;</p> | <p align="center">&#x2713;</p> |
|[Azure Sentinel](https://docs.microsoft.com/azure/sentinel/quickstart-get-visibility) **(предварительная версия)**| <p align="center">&#x2713;</p> | <p align="center"> [Уведомление о проблеме](https://github.com/microsoftgraph/security-api-solutions/issues/new) </p> | <p align="center"> [Уведомление о проблеме](https://github.com/microsoftgraph/security-api-solutions/issues/new) </p> |
|[Palo Alto Networks](https://docs.paloaltonetworks.com/pan-os/9-0/pan-os-web-interface-help/monitor/monitor-logs/log-types.html)| <p align="center">&#x2713;</p> | <p align="center"> [Уведомление о проблеме](https://github.com/microsoftgraph/security-api-solutions/issues/new) </p> | <p align="center"> [Уведомление о проблеме](https://github.com/microsoftgraph/security-api-solutions/issues/new) </p> |
> **Примечание.** К экосистеме безопасности Microsoft Graph постоянно подключаются новые поставщики. Чтобы запросить новых поставщиков или дополнительную поддержку у существующих поставщиков, [уведомите о проблеме в репозитории GitHub для Microsoft Graph Security](https://github.com/microsoftgraph/security-api-solutions/issues/new).

## <a name="common-use-cases"></a>Основные варианты использования

Ниже приводятся некоторые из наиболее популярных запросов для работы с Microsoft Graph Security API.

| **Варианты использования**   | **Ресурсы REST** | **Попробовать в песочнице Graph** |
|:---------------|:--------|:----------|
| Перечисление оповещений | [Перечисление оповещений](../api/alert-list.md) | [https://graph.microsoft.com/v1.0/security/alerts](https://developer.microsoft.com/graph/graph-explorer?request=security/alerts&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com) |
| Обновление оповещений | [Обновление оповещения](../api/alert-update.md) | [https://graph.microsoft.com/v1.0/security/alerts/{alert-id}](https://developer.microsoft.com/graph/graph-explorer?request=security/alerts/{alert-id}&method=PATCH&version=v1.0&GraphUrl=https://graph.microsoft.com) |

Можно использовать [веб-перехватчиков](/graph/webhooks) Microsoft Graph, чтобы подписаться на получение уведомлений об обновлениях объектов системы безопасности Microsoft Graph.

## <a name="resources"></a>Ресурсы

Создавайте код и внесите вклад в примеры Microsoft Graph Security API:

- [Пример для ASP.NET (C#)](https://github.com/microsoftgraph/aspnet-security-api-sample)
- [Пример для Python](https://github.com/microsoftgraph/python-security-rest-sample)
- [Пример для Node.js (JavaScript)](https://github.com/microsoftgraph/nodejs-security-sample)

Взаимодействие с сообществом:

- [Присоединяйтесь к сообществу Tech Community](https://aka.ms/graphsecuritycommunity)
- [Обсуждения на сайте StackOverflow](https://stackoverflow.com/questions/tagged/microsoft-graph-security)

## <a name="next-steps"></a>Дальнейшие действия

Microsoft Graph Security API раскрывает новые способы взаимодействия с решениями для обеспечения безопасности от корпорации Майкрософт и партнеров. Чтобы приступить к работе, следуйте указанным ниже инструкциям.

- Подробно изучите [оповещения](alert.md).
- Опробуйте API в [песочнице Graph](https://developer.microsoft.com/graph/graph-explorer). В разделе **Примеры запросов** выберите элемент **Показать другие примеры** и установите категорию безопасности в положение **Вкл.**
- Попробуйте [подписаться на получение уведомлений](/graph/webhooks) об изменениях объекта.

Нужны идеи? Посмотрите, [как наши партнеры используют Microsoft Graph](https://developer.microsoft.com/graph/graph/examples#partners).

## <a name="see-also"></a>См. также

[Создавайте код и внесите вклад](https://github.com/microsoftgraph/security-api-solutions/blob/master/CONTRIBUTING.md) в примеры Microsoft Graph Security API:

- [Пример для ASP.NET (C#)](https://github.com/microsoftgraph/aspnet-security-api-sample)
- [Пример для Python](https://github.com/microsoftgraph/python-security-rest-sample)
- [Пример для Node.js (JavaScript)](https://github.com/microsoftgraph/nodejs-security-sample)
- [Пример для PowerShell](https://aka.ms/graphsecuritypowershellsample)
- [Другие примеры или добавление нового примера](https://aka.ms/graphsecurityapicode)

Ознакомьтесь с другими возможностями подключения с помощью Microsoft Graph Security API:

- [Соединители Microsoft Graph Security для Logic Apps, Flow и PowerApps](https://aka.ms/graphsecurityconnectors)
- [Соединитель Microsoft Graph Security для Power BI](https://aka.ms/graphsecuritypowerbiconnectordoc)
- [Примеры записных книжек Jupyter](https://aka.ms/graphsecurityjupyternotebooks)

Взаимодействие с сообществом:

- [Присоединяйтесь к сообществу Tech Community](https://aka.ms/graphsecuritycommunity)
- [Обсуждения на сайте StackOverflow](https://stackoverflow.com/questions/tagged/microsoft-graph-security)