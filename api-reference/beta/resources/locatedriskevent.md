---
title: Тип ресурса Локатедрискевент
description: Событие риска, обнаруженное защитой удостоверений Azure Active Directory на основе данных о расположении. К найденным относятся следующие типы событий риска.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: cloudhandler
ms.openlocfilehash: 4fbad6d2b2cc736167f313ad6f70b8f0aea2e63b
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46806564"
---
# <a name="locatedriskevent-resource-type"></a>Тип ресурса Локатедрискевент

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Событие риска, обнаруженное [защитой удостоверений Azure Active Directory](https://azure.microsoft.com/documentation/articles/active-directory-identityprotection/) на основе данных о расположении. К найденным относятся следующие типы событий риска.
* [входы с анонимными IP-адресами](anonymousipriskevent.md)
* [входы с зараженных вредоносными программами устройств](malwareriskevent.md)
* [невозможность перемещаться к необычным расположениям](impossibletravelriskevent.md)
* [входы из подозрительных IP-адресов](suspiciousipriskevent.md)
* [входы из незнакомых расположений](unfamiliarlocationriskevent.md) Полную информацию о событиях риска можно найти в [документации по защите удостоверений Azure AD](https://azure.microsoft.com/documentation/articles/active-directory-identityprotection-risk-events-types/).


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение Локатедрискевент](../api/locatedriskevent-get.md) | [локатедрискевент](locatedriskevent.md) |Чтение свойств и связей объекта Локатедрискевент.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|closedDateTime|dateTimeOffset| Дата и время закрытия события риска|
|createdDateTime|dateTimeOffset| Дата и время создания события риска. Он всегда больше или равен значению DateTime самого события риска. Это правильное свойство, используемое в качестве фильтра при запросе событий риска.|
|id|string| Только для чтения|
|ipAddress|string| IP-адрес входа|
|location|string| Расположение, подключенное к IP-адресу входа|
|рискевентдатетиме|dateTimeOffset| Дата и время возникновения события риска|
|рискевентстатус|string| Возможные значения: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.|
|riskLevel|string| Возможные значения: `low`, `medium`, `high`.|
|рискевенттипе|string| Тип риска|
|userDisplayName|string| Имя пользователя под угрозой|
|userId|строка| Идентификатор пользователя, который подвергается риску|
|userPrincipalName|string| Имя участника пользователя, который подвергается риску|

## <a name="relationships"></a>Отношения
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|импактедусер|[user](user.md)| Только для чтения. Допускается значение null.|

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
