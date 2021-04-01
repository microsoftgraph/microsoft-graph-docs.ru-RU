---
title: тип ресурса locatedRiskEvent
description: 'Событие риска, обнаруженное Azure Active Directory Identity Protection, основанное на данных расположения. Типы событий, связанных с расположенными рисками, включают:'
localization_priority: Normal
doc_type: resourcePageType
ms.prod: identity-and-sign-in
author: cloudhandler
ms.openlocfilehash: c53c503132a0b280c8b7fb02c99816d2ee7a5f03
ms.sourcegitcommit: c7776e5659c391e7c9ce1cd46e242a5ddc38dba2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/01/2021
ms.locfileid: "51490993"
---
# <a name="locatedriskevent-resource-type"></a>тип ресурса locatedRiskEvent

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Событие риска, обнаруженное [Azure Active Directory Identity Protection,](/azure/active-directory/identity-protection/overview-identity-protection) основанное на данных расположения. Типы событий, связанных с расположенными рисками, включают:
* [входы с анонимных IP-адресов](anonymousipriskevent.md)
* [входы с устройств, зараженных вредоносными программами](malwareriskevent.md)
* [невозможное путешествие в нетипичные расположения](impossibletravelriskevent.md)
* [входы с подозрительных IP-адресов](suspiciousipriskevent.md)
* [входы из незнакомых мест](unfamiliarlocationriskevent.md) Полные сведения о событиях риска можно найти в документации [azure AD Identity Protection.](/azure/active-directory/identity-protection/overview-identity-protection)


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Get locatedRiskEvent](../api/locatedriskevent-get.md) | [locatedRiskEvent](locatedriskevent.md) |Чтение свойств и связей объекта locatedRiskEvent.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|closedDateTime|dateTimeOffset| Дата и время закрытия события риска|
|createdDateTime|dateTimeOffset| Дата и время создания события риска. Это всегда больше или равно дате самого события риска. Это правильное свойство, используемее в качестве фильтра при запросе событий риска.|
|id|string| Только для чтения|
|ipAddress|string| IP-адрес входного|
|location|string| Расположение, прикрепленное к IP-адресу входного|
|riskEventDateTime|dateTimeOffset| Дата и время возникновения события риска|
|riskEventStatus|string| Возможные значения: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.|
|riskLevel|string| Возможные значения: `low`, `medium`, `high`.|
|riskEventType|string| Тип риска|
|userDisplayName|string| Имя пользователя, на которого существует риск|
|userId|строка| ID пользователя, на который существует риск|
|userPrincipalName|string| Основное имя пользователя пользователя, на которого существует риск|

## <a name="relationships"></a>Связи
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|impactedUser|[user](user.md)| Только для чтения. Допускается значение null.|

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
   "abstract": true,
   "keyProperty": "id",
   "baseType":"microsoft.graph.identityRiskEvent",
  "@odata.type": "microsoft.graph.locatedRiskEvent"
}-->

```json
{
  "closedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "id": "string (identifier)",
  "ipAddress": "string",
  "location": "string",
  "riskEventDateTime": "String (timestamp)",
  "riskEventStatus": "string",
  "riskLevel": "string",
  "riskType": "string",
  "userDisplayName": "string",
  "userId": "string",
  "userPrincipalName": "string",
  "riskEventType": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "locatedRiskEvent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->