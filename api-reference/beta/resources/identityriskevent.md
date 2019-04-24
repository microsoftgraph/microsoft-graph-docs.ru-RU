---
title: Тип ресурса Идентитирискевент
description: 'Событие риска, обнаруженное защитой удостоверений Azure Active Directory. Это базовый тип для каждого конкретного типа событий риска:'
author: cloudhandler
localization_priority: Normal
ms.prod: security
ms.openlocfilehash: b5c36ab898805c0638cc199ff8cfb893444f04ec
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32506402"
---
# <a name="identityriskevent-resource-type"></a>Тип ресурса Идентитирискевент

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Событие риска, обнаруженное [защитОй удостоверенИй Azure Active Directory](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/). Это базовый тип для каждого конкретного типа событий риска:

| Тип события         | Описание|
|:---------------|:-----------|
|[Анонимаусиприскевент](anonymousipriskevent.md) | Входы из анонимных IP-адресов. |
|[Малварерискевент](malwareriskevent.md) | Входы с зараженных вредоносными программами устройств. |
|[Импоссиблетравелрискевент](impossibletravelriskevent.md) | НеВозможность перемещаться к необычным расположениям. |
|[Леакедкредентиалсрискевент](leakedcredentialsriskevent.md) | Пользователи с потерянными учетными данными. |
|[СуспиЦиаусиприскевент](suspiciousipriskevent.md) | Входы из подозрительных IP-адресов. |
|[Унфамилиарлокатионрискевент](unfamiliarlocationriskevent.md) | Входы из незнакомых расположений. |

Полную информацию о событиях риска можно найти в [документации по защите удостоверенИй Azure AD](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-reporting-risk-events).

## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение объекта identityRiskEvent](../api/identityriskevent-get.md) | [Идентитирискевент](identityriskevent.md) |Чтение свойств и связей объекта Идентитирискевент.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|Клоседдатетиме|dateTimeOffset| Дата и время закрытия события риска|
|createdDateTime|dateTimeOffset| Дата и время создания события риска. Он всегда больше или равен значению DateTime самого события риска. Это правильное свойство, используемое в качестве фильтра при запросе событий риска.|
|id|строка| Только для чтения|
|Рискевентдатетиме|dateTimeOffset| Дата и время возникновения события риска|
|Рискевентстатус|строка| Возможные значения: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.|
|riskLevel|string| Возможные значения: `low`, `medium`, `high`.|
|Рискевенттипе|строка| Тип риска|
|userDisplayName|строка| Имя пользователя под угрозой|
|userId|строка| Идентификатор пользователя, который подвергается риску|
|userPrincipalName|string| Имя участника пользователя, который подвергается риску|

## <a name="relationships"></a>Связи
| Отношение | Тип   |Описание|
|:---------------|:--------|:----------|
|Импактедусер|[user](user.md)| Только для чтения. Допускается значение null.|

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON. 

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.identityRiskEvent"
}-->

```json
{
  "closedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "id": "string (identifier)",
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
  "description": "identityRiskEvent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/identityriskevent.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
