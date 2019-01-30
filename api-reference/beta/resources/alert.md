---
title: Тип оповещения ресурса
description: Представляет потенциальных проблем безопасности в клиент пользователя, который идентификации Майкрософт или партнер решения по обеспечению безопасности. Используйте оповещения для объединения и упростить управление проблемами безопасности через все интегрированные решения. Примеры запросов в обозревателе график Дополнительные сведения см.
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: c7973522b8593d38724ee40374f40d58d3408ff6
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/30/2019
ms.locfileid: "29642403"
---
# <a name="alert-resource-type"></a>Тип оповещения ресурса

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет потенциальных проблем безопасности в клиент пользователя, который идентификации Майкрософт или партнер решения по обеспечению безопасности. Используйте оповещения для объединения и упростить управление проблемами безопасности через все интегрированные решения. Примеры запросов в [Обозревателе график](https://developer.microsoft.com/graph/graph-explorer)Дополнительные сведения см.

Оповещения можно извлечь из списка в разделе [Общие сведения о безопасности Microsoft Graph](security-api-overview.md)поставщиков безопасности.

## <a name="methods"></a>Методы

| Метод   | Возвращаемый тип|Описание|
|:---------------|:--------|:----------|
|[получение оповещения](../api/alert-get.md); | [оповещения](alert.md) |Чтение свойства и связи оповещения объекта.|
|[обновление оповещения](../api/alert-update.md). | [оповещения](alert.md) |Обновление оповещений объекта. |
|[перечисление оповещений](../api/alert-list.md); | [оповещение о](alert.md) семейства сайтов |Получите коллекцию объекта оповещения.|

## <a name="properties"></a>Свойства

| Свойство   | Тип|Описание|
|:---------------|:--------|:----------|
|activityGroupName|String|Имя или псевдоним группы активности (злоумышленник) относится это предупреждение.|
|assignedTo|String|Имя аналитик оповещение будет назначен для рассмотрения расследования и исправлению (поддерживает [обновление](../api/alert-update.md)).|
|azureSubscriptionId|String|Идентификатор подпиской Azure, этот параметр указан, если это предупреждение связано с Azure ресурсов.|
|azureTenantId |String|Идентификатор Azure Active Directory клиента. Обязательный. |
|category|String|Категория оповещения (например, credentialTheft, ransomware, и т.д.).|
|closedDateTime|DateTimeOffset|Время закрытия оповещение. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, полночь UTC 1 января 2014 г будет выглядеть следующим образом: `'2014-01-01T00:00:00Z'` (поддерживает [обновление](../api/alert-update.md)).|
|cloudAppStates|[cloudAppSecurityState](cloudappsecuritystate.md) коллекции|Связанные с безопасностью информацию о состояниях созданный поставщиком об облачных приложений в секунду связанных с этой проблемой.|
|comments|Коллекция String|Предоставленный заказчиком комментарии на оповещения (для управления предупреждениями клиента) (поддерживает [обновление](../api/alert-update.md)).|
|confidence|Int32|Достоверные логика обнаружения (от 1 до 100 процентов).|
|createdDateTime |DateTimeOffset|Время, в которой был создан оповещение оповещения поставщиком. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`. Обязательный.|
|description|String|Описание оповещения.|
|detectionIds|Коллекция String|Набор предупреждений, связанных с этой сущности оповещения (каждого оповещения помещается SIEM как отдельную запись).|
|eventDateTime |DateTimeOffset|Время возникновения события, который был триггеров для создания оповещения. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`. Обязательный.|
|свои отзывы и предложения|alertFeedback|Отзыв аналитик на оповещение. Возможные значения: `unknown`, `truePositive`, `falsePositive`, `benignPositive`. (поддерживает [обновление](../api/alert-update.md))|
|fileStates|[fileSecurityState](filesecuritystate.md) коллекции|Связанные с безопасностью информацию о состояниях созданный поставщиком о файлов, связанных с этой проблемой.|
|hostStates|[hostSecurityState](hostsecuritystate.md) коллекции|Связанные с безопасностью информацию о состояниях созданный поставщиком о узлами, связанных с этой проблемой.|
|id |String|GUID/уникальный идентификатор, созданный поставщика. Только для чтения. Обязательный.|
|lastModifiedDateTime|DateTimeOffset|Время последнего изменения оповещений сущности. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.|
|malwareStates|[malwareState](malwarestate.md) коллекции|Анализ угроз, относящиеся к вредоносных программ, связанных с этой проблемой.|
|networkConnections|[networkConnection](networkconnection.md) семейства сайтов|Связанные с безопасностью информацию о состояниях созданный поставщиком о сетевых соединений, связанных с этой проблемой.|
|процессы|[Коллекция](process.md)|Связанные с безопасностью информацию о состояниях созданный поставщиком о процесса или процессов, связанных с этой проблемой.|
|recommendedActions|Коллекция String|Поставщик/поставщика рекомендуется необходимые действия из-за оповещения (например, изоляция компьютера, enforce2FA, reimage узла).|
|registryKeyStates|[registryKeyState](registrykeystate.md) коллекции|Связанные с безопасностью информацию о состояниях созданный поставщиком о разделах реестра, связанных с этой проблемой.|
|уровень серьезности |alertSeverity|Серьезность оповещения — задание с поставщиком/поставщика. Возможные значения: `unknown`, `informational`, `low`, `medium`, `high`. Обязательный.|
|sourceMaterials|Коллекция String|Гиперссылки (URI) для исходного материала связанные с оповещение, например, пользовательского интерфейса поставщика для оповещений и журнал поиска, и т.д.|
|status |alertStatus|Состояние оповещений жизненного цикла (рабочей области). Возможные значения: `unknown`, `newAlert`, `inProgress`, `resolved`. (поддерживает [обновление](../api/alert-update.md)). Обязательный.|
|tags|Коллекция String|Определяемые пользователем меток, которые могут применяться к оповещения и может выступать в качестве условий фильтра (например «HVA», «ЗАФИКСИРОВАЛА», и т.д.) (поддерживает [обновление](../api/alert-update.md)).|
|title |String|Название оповещения. Обязательный.|
|триггеры|[alertTrigger](alerttrigger.md) коллекции|Связанные с безопасностью сведения об определенных свойств, которые запускаются оповещения (свойств, появляющихся в оповещении о). Уведомления могут содержать сведения о нескольких пользователей, узлы, файлы, IP-адреса. Это поле указывает, какие свойства инициирующую создания оповещений.|
|userStates|[userSecurityState](usersecuritystate.md) коллекции|Связанные с безопасностью информацию о состояниях созданный поставщиком об учетных записях пользователей, связанных с этой проблемой.|
|vendorInformation |[securityVendorInformation](securityvendorinformation.md)|Сложный тип, содержащий сведения о безопасности продуктов и услуг поставщика, поставщик и subprovider (например, поставщика = Майкрософт; поставщика = ATP Защитник Windows; subProvider = AppLocker). Обязательный.|
|vulnerabilityStates|[vulnerabilityState](vulnerabilitystate.md) коллекции|Анализ угроз, относящиеся к одной или нескольких уязвимостей, связанных с этой проблемой.|

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.alert"
}-->

```json
{
  "activityGroupName": "String",
  "assignedTo": "String",
  "azureSubscriptionId": "String",
  "azureTenantId": "String",
  "category": "String",
  "closedDateTime": "String (timestamp)",
  "cloudAppStates": [{"@odata.type": "microsoft.graph.cloudAppSecurityState"}],
  "comments": ["String"],
  "confidence": 1024,
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "detectionIds": ["String"],
  "eventDateTime": "String (timestamp)",
  "feedback": "@odata.type: microsoft.graph.alertFeedback",
  "fileStates": [{"@odata.type": "microsoft.graph.fileSecurityState"}],
  "hostStates": [{"@odata.type": "microsoft.graph.hostSecurityState"}],
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "malwareStates": [{"@odata.type": "microsoft.graph.malwareState"}],
  "networkConnections": [{"@odata.type": "microsoft.graph.networkConnection"}],
  "processes": [{"@odata.type": "microsoft.graph.process"}],
  "recommendedActions": ["String"],
  "registryKeyStates": [{"@odata.type": "microsoft.graph.registryKeyState"}],
  "severity": "@odata.type: microsoft.graph.alertSeverity",
  "sourceMaterials": ["String"],
  "status": "@odata.type: microsoft.graph.alertStatus",
  "tags": ["String"],
  "title": "String",
  "triggers": [{"@odata.type": "microsoft.graph.alertTrigger"}],
  "userStates": [{"@odata.type": "microsoft.graph.userSecurityState"}],
  "vendorInformation": {"@odata.type": "microsoft.graph.securityVendorInformation"},
  "vulnerabilityStates": [{"@odata.type": "microsoft.graph.vulnerabilityState"}]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "alert resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/alert.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
