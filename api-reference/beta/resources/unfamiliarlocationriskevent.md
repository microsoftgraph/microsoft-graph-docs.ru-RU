---
title: Тип ресурса unfamiliarLocationRiskEvent
description: Событие риск, обнаруженных защитой Azure Active Directory Identity которых учетной записи входа в предпринимается попытка из новое расположение для этого пользователя. Полные сведения о событиях риска можно найти в документации по Azure AD защиту.
localization_priority: Normal
ms.openlocfilehash: adad214c0ac58540f1115b836c2c5f26faa6c031
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29507980"
---
# <a name="unfamiliarlocationriskevent-resource-type"></a>Тип ресурса unfamiliarLocationRiskEvent

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Событие риск, обнаруженных с [Azure Active Directory защиту](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/) , где учетной записи входа в предпринимается попытка из новое расположение для этого пользователя. Полные сведения о событиях риска можно найти в [документации по Azure AD защиту](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection-risk-events-types/).


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение unfamiliarLocationRiskEvent](../api/unfamiliarlocationriskevent-get.md) | [unfamiliarLocationRiskEvent](unfamiliarlocationriskevent.md) |Чтение свойства и связи объекта unfamiliarLocationRiskEvent.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|closedDateTime|dateTimeOffset| Дата и время закрытия события риска|
|createdDateTime|dateTimeOffset| Дата и время создания события риска. Это всегда больше или равно datetime самого события риска. Это правильное свойство для использования в качестве фильтра при запросе события рисков.|
|id|string| Только чтение|
|ipAddress|string| IP-адрес входа в|
|location|string| Расположение, подключенного к IP-адрес входа в|
|riskEventDateTime|dateTimeOffset| Дата и время возникновения события риска|
|riskEventStatus|string| Возможные значения: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.|
|riskLevel|string| Возможные значения: `low`, `medium`, `high`.|
|riskEventType|string| Тип риска|
|userDisplayName|string| Имя пользователя в группу риска|
|userId|string| Идентификатор пользователя в группу риска|
|userPrincipalName|string| Имя участника-пользователя пользователя в группу риска|

## <a name="relationships"></a>Отношения
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|impactedUser|[user](user.md)| Только для чтения. Допускается значение null.|

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.unfamiliarLocationRiskEvent"
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
  "userPrincipalName": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "unfamiliarLocationRiskEvent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/unfamiliarlocationriskevent.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
