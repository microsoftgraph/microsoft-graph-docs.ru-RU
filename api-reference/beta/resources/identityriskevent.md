---
title: Тип ресурса Идентитирискевент
description: 'Событие риска, обнаруженное защитой удостоверений Azure Active Directory. Это базовый тип для каждого конкретного типа событий риска:'
author: cloudhandler
localization_priority: Normal
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 079f02b37304a17d370bb3b93fe1cdbda1f4a42c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42496616"
---
# <a name="identityriskevent-resource-type"></a>Тип ресурса Идентитирискевент

Пространство имен: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

>[!NOTE]
>API **идентитирискевентс** устарел и не возвращает данные на 10 января 2020. Дополнительные сведения см. [в разделе устаревшее API идентитирискевентс](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).

Событие риска, обнаруженное [защитой удостоверений Azure Active Directory](https://azure.microsoft.com/documentation/articles/active-directory-identityprotection/). Это базовый тип для каждого конкретного типа событий риска:

| Тип события         | Описание|
|:---------------|:-----------|
|[анонимаусиприскевент](anonymousipriskevent.md) | Входы из анонимных IP-адресов. |
|[малварерискевент](malwareriskevent.md) | Входы с зараженных вредоносными программами устройств. |
|[импоссиблетравелрискевент](impossibletravelriskevent.md) | Невозможность перемещаться к необычным расположениям. |
|[леакедкредентиалсрискевент](leakedcredentialsriskevent.md) | Пользователи с потерянными учетными данными. |
|[суспиЦиаусиприскевент](suspiciousipriskevent.md) | Входы из подозрительных IP-адресов. |
|[унфамилиарлокатионрискевент](unfamiliarlocationriskevent.md) | Входы из незнакомых расположений. |

Полную информацию о событиях риска можно найти в [документации по защите удостоверений Azure AD](/azure/active-directory/active-directory-reporting-risk-events).

## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение объекта identityRiskEvent](../api/identityriskevent-get.md) | [идентитирискевент](identityriskevent.md) |Чтение свойств и связей объекта Идентитирискевент.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|closedDateTime|dateTimeOffset| Дата и время закрытия события риска|
|createdDateTime|dateTimeOffset| Дата и время создания события риска. Он всегда больше или равен значению DateTime самого события риска. Это правильное свойство, используемое в качестве фильтра при запросе событий риска.|
|id|string| Только для чтения|
|рискевентдатетиме|dateTimeOffset| Дата и время возникновения события риска|
|рискевентстатус|строка| Возможные значения: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.|
|riskLevel|string| Возможные значения: `low`, `medium`, `high`.|
|рискевенттипе|строка| Тип риска|
|userDisplayName|строка| Имя пользователя под угрозой|
|userId|строка| Идентификатор пользователя, который подвергается риску|
|userPrincipalName|string| Имя участника пользователя, который подвергается риску|

## <a name="relationships"></a>Связи
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|импактедусер|[user](user.md)| Только для чтения. Допускается значение null.|

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "keyProperty":"id",
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
  "userPrincipalName": "string",
  "riskEventType": "string"
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
  "suppressions": []
}
-->
