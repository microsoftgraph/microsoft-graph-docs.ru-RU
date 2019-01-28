---
title: Использование Microsoft Graph Security API
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
localization_priority: Priority
author: preetikr
ms.prod: security
ms.openlocfilehash: cd55b2d26d7460e7421b9da19658990b53dd7580
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/26/2019
ms.locfileid: "29571697"
---
# <a name="use-the-microsoft-graph-security-api"></a>Использование Microsoft Graph Security API

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Microsoft Graph Security API обеспечивает единый интерфейс и схему интеграции с решениями безопасности от корпорации Майкрософт и партнеров экосистемы. Это позволяет клиентам упростить операции, связанные с безопасностью, и лучше защититься от возрастающих киберугроз. Microsoft Graph Security API можно использовать в качестве службы агрегирования федеративных данных о безопасности, чтобы отправлять запросы всем подключенным поставщикам безопасности для получения агрегированных откликов. Используйте Microsoft Graph Security API для создания приложений с указанными ниже возможностями.

- объединение и корреляция оповещений системы безопасности из нескольких источников;
- разблокировка контекстных данных для получения сведений при расследованиях;
- автоматизация операций безопасности для повышения эффективности;
- обеспечение видимости данных безопасности, чтобы использовать профилактическое управление рисками.

Microsoft Graph Security API включает указанные ниже ключевые объекты.

## <a name="alerts"></a>Оповещения

Оповещения — это потенциальные проблемы безопасности в клиенте пользователя, выявленные решениями по обеспечению безопасности корпорации Майкрософт или партнеров и помеченные для действия или уведомления. С помощью объекта [alerts](alert.md) Microsoft Graph Security можно объединить и оптимизировать устранение проблем безопасности во всех интегрированных решениях. Это также позволит приложениям коррелировать оповещения и контекст для улучшения защиты от угроз и отклика на них. Эти раскрывает операционную эффективность системы безопасности, уменьшая время исследования и время разрешения инцидентов. Благодаря функции обновления оповещений можно синхронизировать состояние определенных оповещений в разных продуктах и службах обеспечения безопасности, интегрированных с Microsoft Graph Security API, с помощью обновления объекта [alerts](alert.md).

Решения, интегрированные с системой безопасности Microsoft Graph, получают уведомления от указанных ниже поставщиков безопасности:

- [Центр безопасности Azure](https://docs.microsoft.com/azure/security-center/security-center-alerts-type)
- [Защита идентификации Azure Active Directory](https://docs.microsoft.com/azure/active-directory/identity-protection/playbook)
- [Microsoft Cloud App Security](https://docs.microsoft.com/cloud-app-security/monitor-alerts )
- [Advanced Threat Protection в Защитнике Windows](https://docs.microsoft.com/windows/security/threat-protection/windows-defender-atp/attack-simulations-windows-defender-advanced-threat-protection)
- [Azure Information Protection](https://docs.microsoft.com/azure/information-protection/faqs#i-see-azure-information-protection-is-listed-as-a-security-provider-for-microsoft-graph-securityhow-does-this-work-and-what-alerts-will-i-receive) **(предварительная версия)**
- Microsoft Intune **(закрытая предварительная версия)**
- Office 365 **(ожидается в ближайшее время)**
- Расширенная защита от угроз Azure **(ожидается в ближайшее время)**
- Решения партнеров, например платформа приложений Palo Alto Networks

> **Примечание.** К экосистеме безопасности Microsoft Graph постоянно подключаются новые поставщики.

## <a name="secure-score-preview"></a>Оценка безопасности (предварительная версия)

[Оценка безопасности (Майкрософт)](https://techcommunity.microsoft.com/t5/Security-Privacy-and-Compliance/Office-365-Secure-Score-is-now-Microsoft-Secure-Score/ba-p/182358) — это решение аналитики безопасности, обеспечивающее обзор вашего набора решений безопасности и способов его улучшения. С помощью одной оценки можно лучше понять, что сделано для снижения риска в решениях Майкрософт. Также можно сравнить свою оценку с другими организациями и просмотреть ее изменение со временем. Объекты [secureScore](securescores.md) и [secureScoreControlProfile](securescorecontrolprofiles.md) системы безопасности Microsoft Graph помогают обеспечить баланс между требованиями по безопасности и производительности в организации, позволяя совмещать соответствующие функции безопасности. Вы также можете спрогнозировать значение оцени после внедрения функций безопасности.

## <a name="common-use-cases"></a>Основные варианты использования

Ниже приводятся некоторые из наиболее популярных запросов для работы с Microsoft Graph Security API.

| **Варианты использования**   | **Ресурсы REST** | **Попробовать в песочнице Graph** |
|:---------------|:--------|:----------|
| Перечисление оповещений | [Перечисление оповещений](../api/alert-list.md) | [https://graph.microsoft.com/beta/security/alerts](https://developer.microsoft.com/graph/graph-explorer?request=security/alerts&method=GET&version=beta&GraphUrl=https://graph.microsoft.com) |
| Обновление оповещений | [Обновление оповещения](../api/alert-update.md) | [https://graph.microsoft.com/beta/security/alerts/{alert-id}](https://developer.microsoft.com/graph/graph-explorer?request=security/alerts/{alert-id}&method=PATCH&version=beta&GraphUrl=https://graph.microsoft.com) |
|Перечисление оценок безопасности|[Перечисление secureScores](../api/securescores-list.md) (предварительная версия)|[https://graph.microsoft.com/beta/security/secureScores](https://developer.microsoft.com/graph/graph-explorer?request=security/secureScores&method=GET&version=beta&GraphUrl=https://graph.microsoft.com)|
|Перечисление профилей составляющих оценки безопасности|[Перечисление secureScoreControlProfiles](../api/securescorecontrolprofiles-list.md) (предварительная версия)|[https://graph.microsoft.com/beta/security/secureScoreControlProfiles](https://developer.microsoft.com/graph/graph-explorer?request=security/secureScoreControlProfiles&method=GET&version=beta&GraphUrl=https://graph.microsoft.com)|
|Обновление профилей составляющих оценки безопасности|[Обновление secureScoreControlProfiles](../api/securescorecontrolprofiles-update.md) (предварительная версия)|[https://graph.microsoft.com/beta/security/secureScoreControlProfiles/{id}](https://developer.microsoft.com/graph/graph-explorer?request=security/secureScoreControlProfiles/{id}&method=PATCH&version=beta&GraphUrl=https://graph.microsoft.com)|

Можно использовать [веб-перехватчиков](/graph/webhooks) Microsoft Graph, чтобы подписаться на получение уведомлений об обновлениях объектов системы безопасности Microsoft Graph.

## <a name="next-steps"></a>Дальнейшие действия

Microsoft Graph Security API раскрывает новые способы взаимодействия с решениями для обеспечения безопасности от корпорации Майкрософт и партнеров. Чтобы приступить к работе, следуйте указанным ниже инструкциям.

- Подробно изучите [оповещения](alert.md), [secureScore](securescores.md) (предварительная версия) и [secureScoreControlProfile](securescorecontrolprofiles.md) (предварительная версия).
- Опробуйте API в [песочнице Graph](https://developer.microsoft.com/graph/graph-explorer). В разделе **Примеры запросов** выберите элемент **Показать другие примеры** и установите категорию безопасности в положение **Вкл.**
- Попробуйте [подписаться на получение уведомлений](/graph/webhooks) об изменениях объекта.

Нужны идеи? Посмотрите, [как наши партнеры используют Microsoft Graph](https://developer.microsoft.com/graph/graph/examples#partners).

## <a name="see-also"></a>См. также

Создавайте код и внесите вклад в примеры Microsoft Graph Security API:

- [Пример для ASP.NET (C#)](https://github.com/microsoftgraph/aspnet-security-api-sample)
- [Пример для Python](https://github.com/microsoftgraph/python-security-rest-sample)
- [Пример для Node.js (JavaScript)](https://github.com/microsoftgraph/nodejs-security-sample)

Взаимодействие с сообществом:

- [Присоединяйтесь к сообществу Tech Community](https://aka.ms/graphsecuritycommunity)
- [Обсуждения на сайте StackOverflow](https://stackoverflow.com/questions/tagged/microsoft-graph-security)
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/security-api-overview.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
