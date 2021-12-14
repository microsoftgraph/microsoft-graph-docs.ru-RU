---
title: Использование Microsoft Graph Security API
description: Microsoft Graph Security API обеспечивает единый интерфейс и схему интеграции с решениями безопасности от корпорации Майкрософт и партнеров экосистемы.
ms.localizationpriority: high
author: preetikr
ms.prod: security
doc_type: conceptualPageType
ms.openlocfilehash: ca0526b7eb1a044b3ba8ecf95d66a09b30b7d17d
ms.sourcegitcommit: c900d22144429ac7aecae3355a4cdc1987cc4234
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/13/2021
ms.locfileid: "61424695"
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

При использовании Microsoft Graph Security API доступны оповещения от указанных ниже поставщиков. Поддержка для оповещений GET, оповещений PATCH и подписки (с помощью веб-перехватчиков) представлена в приведенной ниже таблице.

| Поставщик безопасности | <p align="center">Оповещение GET</p>| <p align="center">Оповещение PATCH</p>| <p align="center">Подписка на оповещения</p>|
|:------------------|:---------|:-----------|:------------------|
|[Microsoft Defender для облака](/azure/defender-for-cloud/alerts-overview)| <p align="center">&#x2713;</p> | <p align="center">&#x2713;</p> | <p align="center">&#x2713;</p> |
|[Защита идентификации Azure Active Directory](/azure/active-directory/identity-protection/playbook) | <p align="center">&#x2713;</p> | <p align="center">[Уведомление о проблеме](https://github.com/microsoftgraph/security-api-solutions/issues/new) *</p> | <p align="center">&#x2713;</p> |
| [Microsoft Defender for Cloud Apps](/cloud-app-security/monitor-alerts) | <p align="center">&#x2713;</p> | <p align="center">[Уведомление о проблеме](https://github.com/microsoftgraph/security-api-solutions/issues/new) *</p> | <p align="center">&#x2713;</p> |
|[Microsoft Defender для конечной точки](/windows/security/threat-protection/microsoft-defender-atp/attack-simulations) **| <p align="center">&#x2713;</p> | <p align="center">&#x2713;</p> | <p align="center"> [Уведомление о проблеме](https://github.com/microsoftgraph/security-api-solutions/issues/new) </p> |
|[Microsoft Defender для удостоверений](/defender-for-identity/understanding-security-alerts#security-alert-categories) ***| <p align="center">&#x2713;</p> | <p align="center">[Уведомление о проблеме](https://github.com/microsoftgraph/security-api-solutions/issues/new) *</p> | <p align="center">&#x2713;</p> |
|Microsoft 365 <ul><li> [По умолчанию](/office365/securitycompliance/alert-policies#default-alert-policies)</li> <li>[Cloud App Security](/office365/securitycompliance/anomaly-detection-policies-in-ocas)</li><li>Пользовательское оповещение</li></ul> | <p align="center">&#x2713;</p> | <p align="center"> [Уведомление о проблеме](https://github.com/microsoftgraph/security-api-solutions/issues/new) </p> | <p align="center"> [Уведомление о проблеме](https://github.com/microsoftgraph/security-api-solutions/issues/new) </p> |
|[Azure Information Protection](/azure/information-protection/faqs#i-see-azure-information-protection-is-listed-as-a-security-provider-for-microsoft-graph-securityhow-does-this-work-and-what-alerts-will-i-receive) **(предварительная версия)**| <p align="center">&#x2713;</p> | <p align="center">[Уведомление о проблеме](https://github.com/microsoftgraph/security-api-solutions/issues/new) *</p> | <p align="center">&#x2713;</p> |
|[Azure Sentinel](/azure/sentinel/quickstart-get-visibility) **(предварительная версия)**| <p align="center">&#x2713;</p> | <p align="center">Не поддерживается в Azure Sentinel. </p> | <p align="center">&#x2713;</p> |
> **Примечание.** К экосистеме безопасности Microsoft Graph постоянно подключаются новые поставщики. Чтобы запросить новых поставщиков или дополнительную поддержку у существующих поставщиков, [уведомите о проблеме в репозитории GitHub для Microsoft Graph Security](https://github.com/microsoftgraph/security-api-solutions/issues/new).

\* Проблема с файлом: статус оповещения обновляется в интегрированных в API безопасности Microsoft Graph приложениях, но не отображается в интерфейсе управления провайдера.

\*\* Microsoft Defender для конечной точки требует дополнительных [ролей пользователя](/windows/security/threat-protection/microsoft-defender-atp/user-roles) помимо ролей, необходимых для Microsoft Graph Security API. Только пользователи, которым назначены роли как в Microsoft Defender для конечной точки, так и в Microsoft Graph Security API, могут получить доступ к данным Microsoft Defender для конечной точки. Поскольку это ограничение не распространяется на проверку подлинности только для приложений, рекомендуется использовать маркер проверки подлинности только для приложений.

\*\*\* Оповещения Microsoft Defender для удостоверений доступны в рамках интеграции с Microsoft Defender for Cloud Apps. Это означает, что вы будете получать оповещения Microsoft Defender для удостоверений только в том случае, если вы присоединились к комплексному решению SecOps и подключили Microsoft Defender для удостоверений к Microsoft Defender for Cloud Apps. Узнайте больше о том, [как интегрировать Microsoft Defender для удостоверений и Microsoft Defender for Cloud Apps](/defender-for-identity/mcas-integration).

## <a name="information-protection"></a>Защита информации

API оценки угроз Microsoft Graph позволяет организациям оценивать угрозу, возникшую для любого пользователя в клиенте. Благодаря этому пользователи могут сообщать в корпорацию Майкрософт о полученной нежелательной почте, фишинговых URL-адресах и вредоносных вложениях. Результат проверки политики и результат повторного сканирования может помочь администраторам клиента понять заключение сканирования угроз и настроить политику организации.

## <a name="secure-score"></a>Оценка безопасности

[Оценка безопасности (Майкрософт)](https://techcommunity.microsoft.com/t5/Security-Privacy-and-Compliance/A-new-home-and-an-all-new-look-for-Microsoft-Secure-Score/ba-p/529641) — это решение аналитики безопасности, обеспечивающее обзор вашего набора решений безопасности и способов его улучшения. С помощью одной оценки можно лучше понять, что сделано для снижения риска в решениях Майкрософт. Также можно сравнить свою оценку с другими организациями и просмотреть ее изменение со временем. Объекты [secureScore](securescore.md) и [secureScoreControlProfile](securescorecontrolprofile.md) системы безопасности Microsoft Graph помогают обеспечить баланс между требованиями по безопасности и производительности в организации, позволяя совмещать соответствующие функции безопасности. Вы также можете спрогнозировать значение оцени после внедрения функций безопасности.

## <a name="common-use-cases"></a>Основные варианты использования

Ниже приводятся некоторые из наиболее популярных запросов для работы с Microsoft Graph Security API.

| **Варианты использования**   | **Ресурсы REST** | **Попробовать в песочнице Graph** |
|:---------------|:--------|:----------|
| Перечисление оповещений | [Перечисление оповещений](../api/alert-list.md) | [https://graph.microsoft.com/v1.0/security/alerts](https://developer.microsoft.com/graph/graph-explorer?request=security/alerts&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com) |
| Обновление оповещений | [Обновление оповещения](../api/alert-update.md) | [https://graph.microsoft.com/v1.0/security/alerts/{alert-id}](https://developer.microsoft.com/graph/graph-explorer?request=security/alerts/{alert-id}&method=PATCH&version=v1.0&GraphUrl=https://graph.microsoft.com) |
|Список оценок безопасности|[Список объектов secureScore](../api/security-list-securescores.md) |[https://graph.microsoft.com/v1.0/security/secureScores](https://developer.microsoft.com/graph/graph-explorer?request=security/secureScores&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com)|
|Получение оценки безопасности|[Получение объектов secureScore](../api/securescore-get.md) |[https://graph.microsoft.com/v1.0/security/secureScores/{id}](https://developer.microsoft.com/graph/graph-explorer?request=security/secureScores/{id}&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com)|
|Список профилей составляющих оценки безопасности|[Список объектов secureScoreControlProfiles](../api/security-list-securescorecontrolprofiles.md) |[https://graph.microsoft.com/v1.0/security/secureScoreControlProfiles](https://developer.microsoft.com/graph/graph-explorer?request=security/secureScoreControlProfiles&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com)|
|Получение профилей составляющих оценки безопасности|[Получение объектов secureScoreControlProfile](../api/securescorecontrolprofile-get.md) |[https://graph.microsoft.com/v1.0/security/secureScoreControlProfiles/{id}](https://developer.microsoft.com/graph/graph-explorer?request=security/secureScoreControlProfiles/{id}&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com)|
|Обновление профилей составляющих оценки безопасности|[Обновление объектов secureScoreControlProfile](../api/securescorecontrolprofile-update.md) |[https://graph.microsoft.com/v1.0/security/secureScoreControlProfiles/{id}](https://developer.microsoft.com/graph/graph-explorer?request=security/secureScoreControlProfiles/{id}&method=PATCH&version=v1.0&GraphUrl=https://graph.microsoft.com)|


Можно использовать [веб-перехватчиков](/graph/webhooks) Microsoft Graph, чтобы подписаться на получение уведомлений об обновлениях объектов системы безопасности Microsoft Graph.

## <a name="resources"></a>Ресурсы

Создавайте код и внесите вклад в примеры Microsoft Graph Security API:

- [Пример для ASP.NET (C#)](https://github.com/microsoftgraph/aspnet-security-api-sample)
- [Пример для Python](https://github.com/microsoftgraph/python-security-rest-sample)
- [Пример для Node.js (JavaScript)](https://github.com/microsoftgraph/nodejs-security-sample)

Взаимодействие с сообществом:

- [Присоединяйтесь к сообществу Tech Community](https://aka.ms/graphsecuritycommunity)
- [Обсуждения на сайте StackOverflow](https://stackoverflow.com/questions/tagged/microsoft-graph-security)

## <a name="whats-new"></a>Новые возможности
Узнайте о [новых функциях и обновлениях](/graph/whats-new-overview) для этих наборов API.

## <a name="next-steps"></a>Дальнейшие действия

Microsoft Graph Security API раскрывает новые способы взаимодействия с решениями для обеспечения безопасности, предоставляемыми корпорацией Майкрософт и партнерами. Чтобы приступить к работе, следуйте указанным ниже инструкциям.

- Подробно изучите [оповещения](alert.md), объекты [secureScore](securescore.md) и [secureScoreControlProfile](securescorecontrolprofile.md).
- Опробуйте API в [песочнице Graph](https://developer.microsoft.com/graph/graph-explorer). В разделе **Примеры запросов** выберите элемент **Показать другие примеры** и установите категорию безопасности в положение **Вкл.**
- Попробуйте [подписаться на получение уведомлений](/graph/webhooks) об изменениях объекта.

Нужны идеи? Посмотрите, [как наши партнеры используют Microsoft Graph](https://developer.microsoft.com/graph/partners).

## <a name="see-also"></a>См. также

[Создавайте код и внесите вклад](https://github.com/microsoftgraph/security-api-solutions/blob/master/CONTRIBUTING.md) в примеры Microsoft Graph Security API:

- [Пример для ASP.NET (C#)](https://github.com/microsoftgraph/aspnet-security-api-sample)
- [Пример для Python](https://github.com/microsoftgraph/python-security-rest-sample)
- [Пример для Node.js (JavaScript)](https://github.com/microsoftgraph/nodejs-security-sample)
- [Пример для PowerShell](https://aka.ms/graphsecuritypowershellsample)
- [Другие примеры или добавление нового примера](https://aka.ms/graphsecurityapicode)

Ознакомьтесь с другими возможностями подключения с помощью Microsoft Graph Security API:

- [Соединители Microsoft Graph Security для Logic Apps, Flow и Power Apps](https://aka.ms/graphsecurityconnectors)
- [Примеры записных книжек Jupyter](https://aka.ms/graphsecurityjupyternotebooks)

Взаимодействие с сообществом:

- [Присоединяйтесь к сообществу Tech Community](https://techcommunity.microsoft.com/t5/microsoft-graph-security-api/bd-p/SecurityGraphAPI)
- [Обсуждения на сайте StackOverflow](https://stackoverflow.com/questions/tagged/microsoft-graph-security)

