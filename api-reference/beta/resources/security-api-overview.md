---
title: Использование Microsoft Graph Security API
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
localization_priority: Priority
author: preetikr
ms.prod: security
ms.openlocfilehash: d516dc576027034fd08ee9b67b0171d0d0b3b3ad
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32549050"
---
# <a name="use-the-microsoft-graph-security-api"></a>Использование Microsoft Graph Security API

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

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

## <a name="threat-indicators-preview"></a>Индикаторы угроз (предварительная версия)

Индикаторы угроз, также называемые индикаторами компрометации (IoCs), представляют данные об известных угрозах, таких как вредоносные файлы, URL-адреса, домены и IP-адреса. Пользователи могут создавать индикаторы путем сбора внутренней аналитики угроз или получения индикаторов от сообществ по анализу угроз, лицензированных веб-каналов и других источников. Затем эти индикаторы используются в различных средствах безопасности для защиты от соответствующих угроз.

Объект [tiIndicators](tiindicator.md) Microsoft Graph Security позволяет пользователям направлять свои индикаторы в решения по обеспечению безопасности Майкрософт для включения блокировки и оповещений о вредоносных действиях или их разрешения, что приостанавливает действия для индикаторов, считающихся неважными для организации. При отправке индикаторов указывается как решение корпорации Майкрософт, использующее индикатор, так и выполняемое с индикатором действие.

Можно интегрировать объект [tiIndicator](tiindicator.md) в свое приложение или использовать одну из указанных ниже интегрированных платформ аналитики угроз (TIP):

- [Palo Alto Networks MineMeld Threat Intelligence Sharing](https://www.paloaltonetworks.com/products/secure-the-network/subscriptions/minemeld)
- [Платформа аналитики угроз MISP с открытым кодом](http://www.misp-project.org/), доступная в [примере аналитики угроз](https://aka.ms/tipmispsample)

Индикаторы угроз, отправляемые через Microsoft Graph Security API, сейчас доступны в [Azure Sentinel](https://docs.microsoft.com/azure/sentinel/overview) (предварительная версия), что позволяет коррелировать индикаторы угроз с данными журнала для получения оповещений о вредоносных действиях. Поддержка в других службах безопасности Майкрософт, включая брандмауэр Azure, появится в ближайшее время.

## <a name="security-actions-preview"></a>Действия по обеспечению безопасности (предварительная версия)

Принимайте незамедлительные действия по защите от угроз с помощью объекта [securityAction](securityaction.md) Microsoft Graph Security. Если аналитик безопасности обнаруживает новый индикатор, например вредоносный файл, URL-адрес, домен или IP-адрес, можно сразу же включить защиту в решении по обеспечению безопасности от корпорации Майкрософт. Вызывайте действие для определенного поставщика услуг, просматривайте все выполненные действия и отменяйте действие при необходимости. Воспользуйтесь действиями по обеспечению безопасности с помощью [ATP в Защитнике Windows](https://docs.microsoft.com/windows/security/threat-protection/windows-defender-atp/windows-defender-advanced-threat-protection), чтобы заблокировать вредоносную активность в конечных точках Windows с использованием свойств, отображаемых в оповещениях или выявленных при изучении.

  > **Примечание.** В настоящее время действия по обеспечению безопасности поддерживают только разрешения для приложений.

## <a name="secure-score-preview"></a>Оценка безопасности (предварительная версия)

[Оценка безопасности (Майкрософт)](https://techcommunity.microsoft.com/t5/Security-Privacy-and-Compliance/Office-365-Secure-Score-is-now-Microsoft-Secure-Score/ba-p/182358) — это решение аналитики безопасности, обеспечивающее обзор вашего набора решений безопасности и способов его улучшения. С помощью одной оценки можно лучше понять, что сделано для снижения риска в решениях Майкрософт. Также можно сравнить свою оценку с другими организациями и просмотреть ее изменение со временем. Объекты [secureScore](securescores.md) и [secureScoreControlProfiles](securescorecontrolprofiles.md) системы безопасности Microsoft Graph помогают обеспечить баланс между требованиями по безопасности и производительности в организации, позволяя совмещать соответствующие функции безопасности. Вы также можете спрогнозировать значение оцени после внедрения функций безопасности.

## <a name="common-use-cases"></a>Основные варианты использования

Ниже приводятся некоторые из наиболее популярных запросов для работы с Microsoft Graph Security API.

| **Варианты использования**   | **Ресурсы REST** | **Попробовать в песочнице Graph** |
|:---------------|:--------|:----------|
| Перечисление оповещений | [Перечисление оповещений](../api/alert-list.md) | [https://graph.microsoft.com/beta/security/alerts](https://developer.microsoft.com/graph/graph-explorer?request=security/alerts&method=GET&version=beta&GraphUrl=https://graph.microsoft.com) |
| Обновление оповещений | [Обновление оповещения](../api/alert-update.md) </br> [Обновление нескольких оповещений](../api/alert-updatealerts.md) | [https://graph.microsoft.com/beta/security/alerts/{alert-id}](https://developer.microsoft.com/graph/graph-explorer?request=security/alerts/{alert-id}&method=PATCH&version=beta&GraphUrl=https://graph.microsoft.com) </br> [https://graph.microsoft.com/beta/security/alerts/updateAlerts](https://developer.microsoft.com/graph/graph-explorer?request=security/alerts/updateAlerts&method=POST&version=beta&GraphUrl=https://graph.microsoft.com) |
| Получение действия по обеспечению безопасности | [Получение действия по обеспечению безопасности](../api/securityaction-get.md) (предварительная версия)|[https://graph.microsoft.com/beta/security/securityActions/{id}](https://developer.microsoft.com/graph/graph-explorer?request=security/securityActions/{id}&method=GET&version=beta&GraphUrl=https://graph.microsoft.com)|
|Перечисление действий по обеспечению безопасности| [Перечисление действий по обеспечению безопасности](../api/securityactions-list.md) (предварительная версия)|[https://graph.microsoft.com/beta/security/securityActions](https://developer.microsoft.com/graph/graph-explorer?request=security/securityActions&method=GET&version=beta&GraphUrl=https://graph.microsoft.com)|
|Создание действий по обеспечению безопасности|[Создание действий по обеспечению безопасности](../api/securityactions-post.md) (предварительная версия)|[https://graph.microsoft.com/beta/security/securityActions](https://developer.microsoft.com/graph/graph-explorer?request=security/securityActions&method=POST&version=beta&GraphUrl=https://graph.microsoft.com)|
|Отмена действия по обеспечению безопасности|[Отмена действий по обеспечению безопасности](../api/securityaction-cancelsecurityaction.md) (предварительная версия)| [https://graph.microsoft.com/beta/security/securityActions/{id}/cancelSecurityAction](https://developer.microsoft.com/graph/graph-explorer?request=security/securityActions/{id}/cancelSecurityAction&method=POST&version=beta&GraphUrl=https://graph.microsoft.com) |
|Получение индикатора аналитики угроз|[Получение объекта tiIndicator](../api/tiindicator-get.md) (предварительная версия)| [https://graph.microsoft.com/beta/security/tiIndicators/{id}](https://developer.microsoft.com/graph/graph-explorer?request=security/tiIndicators/{id}&method=GET&version=beta&GraphUrl=https://graph.microsoft.com)|
|Перечисление индикаторов аналитики угроз | [Перечисление объектов tiIndicator](../api/tiindicators-list.md) (предварительная версия) | [https://graph.microsoft.com/beta/security/tiIndicators](https://developer.microsoft.com/graph/graph-explorer?request=security/tiIndicators&method=GET&version=beta&GraphUrl=https://graph.microsoft.com)|
|Создание индикатора аналитики угроз|[Создание объекта tiIndicator](../api/tiindicators-post.md) (предварительная версия)|[https://graph.microsoft.com/beta/security/tiIndicators](https://developer.microsoft.com/graph/graph-explorer?request=security/tiIndicators&method=POST&version=beta&GraphUrl=https://graph.microsoft.com)|
|Отправка индикаторов аналитики угроз|[Отправка объектов tiIndicator](../api/tiindicator-submittiindicators.md) (предварительная версия)| [https://graph.microsoft.com/beta/security/tiIndicators/submitTiIndicators](https://developer.microsoft.com/graph/graph-explorer?request=security/tiIndicators/submitTiIndicators&method=POST&version=beta&GraphUrl=https://graph.microsoft.com) |
|Обновление индикаторов аналитики угроз|[Обновление объекта tiIndicator](../api/tiindicator-update.md) (предварительная версия) </br>[Обновление нескольких объектов tiIndicator](../api/tiindicator-updatetiindicators.md) (предварительная версия)| [https://graph.microsoft.com/beta/security/tiIndicators/{id}](https://developer.microsoft.com/graph/graph-explorer?request=security/tiIndicators/{id}&method=POST&version=beta&GraphUrl=https://graph.microsoft.com) </br>[https://graph.microsoft.com/beta/security/tiIndicators/updateTiIndicators](https://developer.microsoft.com/graph/graph-explorer?request=security/tiIndicators/updateTiIndicators&method=POST&version=beta&GraphUrl=https://graph.microsoft.com)|
|Удаление индикаторов аналитики угроз|[Удаление объекта tiIndicator](../api/tiindicator-delete.md) (предварительная версия) </br>[Удаление нескольких объектов tiIndicator](../api/tiindicator-deletetiindicators.md) (предварительная версия) </br>[Удаление объекта tiIndicator по externalId](../api/tiindicator-deletetiindicatorsbyexternalid.md) (предварительная версия)| DELETE </br>[https://graph.microsoft.com/beta/security/tiIndicators/{id}](https://developer.microsoft.com/graph/graph-explorer?request=security/tiIndicators/{id}&method=DELETE&version=beta&GraphUrl=https://graph.microsoft.com) </br>POST</br>[https://graph.microsoft.com/beta/security/tiIndicators/deleteTiIndicators](https://developer.microsoft.com/graph/graph-explorer?request=security/tiIndicators/deleteTiIndicators&method=POST&version=beta&GraphUrl=https://graph.microsoft.com)</br>POST</br>[https://graph.microsoft.com/beta/security/tiIndicators/deleteTiIndicatorsByExternalId](https://developer.microsoft.com/graph/graph-explorer?request=security/tiIndicators/deleteTiIndicatorsByExternalId&method=POST&version=beta&GraphUrl=https://graph.microsoft.com)|
|Перечисление оценок безопасности|[Перечисление secureScores](../api/securescores-list.md) (предварительная версия)|[https://graph.microsoft.com/beta/security/secureScores](https://developer.microsoft.com/graph/graph-explorer?request=security/secureScores&method=GET&version=beta&GraphUrl=https://graph.microsoft.com)|
|Перечисление профилей составляющих оценки безопасности|[Перечисление secureScoreControlProfiles](../api/securescorecontrolprofiles-list.md) (предварительная версия)|[https://graph.microsoft.com/beta/security/secureScoreControlProfiles](https://developer.microsoft.com/graph/graph-explorer?request=security/secureScoreControlProfiles&method=GET&version=beta&GraphUrl=https://graph.microsoft.com)|
|Обновление профилей составляющих оценки безопасности|[Обновление secureScoreControlProfiles](../api/securescorecontrolprofiles-update.md) (предварительная версия)|[https://graph.microsoft.com/beta/security/secureScoreControlProfiles/{id}](https://developer.microsoft.com/graph/graph-explorer?request=security/secureScoreControlProfiles/{id}&method=PATCH&version=beta&GraphUrl=https://graph.microsoft.com)|

Можно использовать [веб-перехватчиков](/graph/webhooks) Microsoft Graph, чтобы подписаться на получение уведомлений об обновлениях объектов Microsoft Graph Security API.

## <a name="next-steps"></a>Дальнейшие действия

Microsoft Graph Security API раскрывает новые способы взаимодействия с решениями для обеспечения безопасности от корпорации Майкрософт и партнеров. Чтобы приступить к работе, следуйте указанным ниже инструкциям.

- Подробно изучите [оповещения](alert.md), [tiIndicator](tiindicator.md) (предварительная версия), [securityAction](securityaction.md) (предварительная версия), [secureScore](securescores.md) (предварительная версия) и [secureScoreControlProfiles](securescorecontrolprofiles.md) (предварительная версия).
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
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/security-api-overview.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
