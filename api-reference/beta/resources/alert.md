---
title: Тип ресурса alert
description: Представляет потенциальные проблемы безопасности в клиенте пользователя, выявленные решениями по обеспечению безопасности корпорации Майкрософт или партнеров. Используйте оповещения, чтобы объединить и оптимизировать управления проблемами безопасности во всех интегрированных решениях. Дополнительные сведения см. в примерах запросов в песочнице Graph.
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 928be5ed3245b19c64cd09a61fea6a1ead0054c7
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722183"
---
# <a name="alert-resource-type"></a>Тип ресурса alert

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет потенциальные проблемы безопасности в клиенте пользователя, выявленные решениями по обеспечению безопасности корпорации Майкрософт или партнеров. Используйте оповещения, чтобы объединить и оптимизировать управления проблемами безопасности во всех интегрированных решениях. Дополнительные сведения см. в примерах запросов в [песочнице Graph](https://developer.microsoft.com/graph/graph-explorer).

Оповещения можно получать от разных поставщиков безопасности, перечисленных в статье [Обзор безопасности Microsoft Graph](security-api-overview.md).

## <a name="methods"></a>Методы

| Метод   | Возвращаемый тип|Описание|
|:---------------|:--------|:----------|
|[Получение оповещения](../api/alert-get.md) | [alert](alert.md) |Чтение свойств и связей объекта alert.|
|[Обновление оповещения](../api/alert-update.md) | [alert](alert.md) |Обновление объекта alert. |
|[Перечисление оповещений](../api/alert-list.md) | Коллекция [alert](alert.md) |Получение коллекции объектов alert.|
|[Обновление оповещений](../api/alert-updatealerts.md)|Коллекция [alert](alert.md)|Обновление нескольких объектов оповещений.|

## <a name="properties"></a>Свойства

| Свойство   | Тип|Описание|
|:---------------|:--------|:----------|
|activityGroupName|String|Имя или псевдоним группы действий (злоумышленник), с которым связано это оповещение.|
|assignedTo|String|Имя аналитика, которому назначено оповещение для рассмотрения, изучения или исправления (поддерживает [обновление](../api/alert-update.md)).|
|azureSubscriptionId|String|Идентификатор подписки Azure, указываемый, если это оповещение связано с ресурсом Azure.|
|azureTenantId |String|Идентификатор клиента Azure Active Directory. Обязательный атрибут. |
|category|String|Категория оповещения (например, credentialTheft, ransomware и т. д.).|
|closedDateTime|DateTimeOffset|Время закрытия оповещения. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, полночь UTC 1 января 2014 г. `2014-01-01T00:00:00Z` (поддерживает [обновление).](../api/alert-update.md)|
|cloudAppStates|Коллекция [cloudAppSecurityState](cloudappsecuritystate.md)|Сведения, связанные с отслеживанием состояния безопасности, созданные поставщиком об облачных приложениях, относящихся к оповещению.|
|comments|Коллекция String|Предоставляемые пользователями комментарии об оповещении (для управления пользовательскими оповещениями) (поддерживает [обновление](../api/alert-update.md)).|
|confidence|Int32|Достоверность логики обнаружения (процентное значение от 1 до 100).|
|createdDateTime |DateTimeOffset|Время создания оповещения поставщиком оповещения. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`. Обязательный атрибут.|
|description|String|Описание оповещения.|
|detectionIds|Коллекция String|Набор оповещений, связанных с объектом оповещения (каждое оповещение передается в SIEM как отдельная запись).|
|eventDateTime |DateTimeOffset|Время возникновения событий, запустивших создание оповещения. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`. Обязательный атрибут.|
|feedback|alertFeedback|Отзыв аналитика об оповещении. Возможные значения: `unknown`, `truePositive`, `falsePositive`, `benignPositive`. (Поддерживает [обновление](../api/alert-update.md))|
|fileStates|Коллекция [fileSecurityState](filesecuritystate.md)|Сведения, связанные с отслеживанием состояния безопасности, созданные поставщиком о файлах, относящихся к оповещению.|
|historyStates|[коллекция alertHistoryState](alerthistorystate.md)| Коллекция **оповещенийHistoryStates,** состоящая из журнала аудита всех обновлений, сделанных в оповещение. |
|hostStates|Коллекция [hostSecurityState](hostsecuritystate.md)|Сведения, связанные с отслеживанием состояния безопасности, созданные поставщиком об узлах, относящихся к оповещению.|
|id |String|GUID или уникальный идентификатор, созданный поставщиком. Только для чтения. Обязательный.|
|incidentIds|Коллекция String|Идентификаторы инцидентов, связанных с текущим оповещением.|
|lastModifiedDateTime|DateTimeOffset|Время последнего изменения объекта оповещения. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|malwareStates|Коллекция [malwareState](malwarestate.md)|Аналитика угроз, относящаяся к вредоносным программам, связанным с оповещением.|
|networkConnections|Коллекция [networkConnection](networkconnection.md)|Сведения, связанные с отслеживанием состояния безопасности, созданные поставщиком о сетевых подключениях, относящихся к оповещению.|
|processes|Коллекция [process](process.md)|Сведения, связанные с отслеживанием состояния безопасности, созданные поставщиком о процессе или процессах, относящихся к оповещению.|
|recommendedActions|Коллекция String|Рекомендуемые поставщиком действия в ответ на оповещение (например, изоляция компьютера, применение двухфакторной проверки подлинности, повторное создание образа узла).|
|registryKeyStates|Коллекция [registryKeyState](registrykeystate.md)|Сведения, связанные с отслеживанием состояния безопасности, созданные поставщиком о разделах реестра, относящихся к оповещению.|
|securityResources|Коллекция [securityResource](securityResource.md)|Ресурсы, связанные с текущим оповещением. Например, для некоторых предупреждений это может быть значение ресурса Azure.|
|severity |alertSeverity|Серьезность оповещения, заданная поставщиком. Возможные значения: `unknown`, `informational`, `low`, `medium`, `high`. Обязательный атрибут.|
|sourceMaterials|Коллекция String|Гиперссылки (URI) на исходные материалы, связанные с оповещением, например пользовательский интерфейс поставщика для оповещений или поиска в журнале и т. д.|
|status |alertStatus|Оповещение о состоянии жизненного цикла (этапа). Возможные значения: `unknown`, `newAlert`, `inProgress`, `resolved`. (Поддерживает [обновление](../api/alert-update.md)). Обязательный атрибут.|
|tags|Коллекция String|Определяемые пользователем метки, которые можно применять к оповещению и использовать в качестве условий фильтра (например, HVA, SAW и т. д.) (поддерживает [обновление](../api/alert-update.md)).|
|title |String|Заголовок оповещения. Обязательный атрибут.|
|triggers|Коллекция [alertTrigger](alerttrigger.md)|Сведения, связанные с безопасностью, об определенных свойствах, запустивших оповещение (свойства, отображаемые в оповещении). Оповещения могут содержать сведения о нескольких пользователях, узлах, файлах, IP-адресах. Это поле указывает, какие свойства запустили создание оповещения.|
|userStates|Коллекция [userSecurityState](usersecuritystate.md)|Сведения, связанные с отслеживанием состояния безопасности, созданные поставщиком об учетных записях пользователей, относящихся к оповещению.|
|vendorInformation |[securityVendorInformation](securityvendorinformation.md)|Сложный тип, содержащий подробные сведения о безопасности продавца продукта или услуги, поставщика субпоставщика (например, продавец = Майкрософт; поставщик = ATP в Защитнике Windows; субпоставщик = AppLocker). Обязательный атрибут.|
|vulnerabilityStates|Коллекция [vulnerabilityState](vulnerabilitystate.md)|Аналитика угроз, относящаяся к одной или нескольким уязвимостям, связанным с оповещением.|

## <a name="relationships"></a>Отношения

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
  "historyStates": [{"@odata.type": "microsoft.graph.alertHistoryState"}],
  "hostStates": [{"@odata.type": "microsoft.graph.hostSecurityState"}],
  "id": "String (identifier)",
  "incidentIds": ["String"],
  "lastModifiedDateTime": "String (timestamp)",
  "malwareStates": [{"@odata.type": "microsoft.graph.malwareState"}],
  "networkConnections": [{"@odata.type": "microsoft.graph.networkConnection"}],
  "processes": [{"@odata.type": "microsoft.graph.process"}],
  "recommendedActions": ["String"],
  "registryKeyStates": [{"@odata.type": "microsoft.graph.registryKeyState"}],
  "securityResources": [{"@odata.type": "microsoft.graph.securityResource"}],
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
  "suppressions": []
}
-->


