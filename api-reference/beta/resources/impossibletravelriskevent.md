---
title: Тип ресурса Импоссиблетравелрискевент
description: Событие риска, обнаруженное службой удостоверений Azure Active Directory, в котором два входа с учетной записью происходят из расположений нетипично для пользователя, и вы не сможете перемещаться между расположениями в период между входами. полная информация события риска можно найти в документации по защите удостоверений Azure AD.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 2b66755924022b4fa30637cc8e97c4f944ad2d79
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36005774"
---
# <a name="impossibletravelriskevent-resource-type"></a>Тип ресурса Импоссиблетравелрискевент

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Событие риска, обнаруженное службой [удостоверений Azure Active Directory](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/) , в котором два входа учетной записи происходят из расположений, нетипичных для пользователя, и вы не сможете перемещаться между расположениями в промежутке между входами. Complete сведения о событиях риска можно найти в [документации по защите удостоверений Azure AD](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection-risk-events-types/).


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение объекта impossibleTravelRiskEvent](../api/impossibletravelriskevent-get.md) | [Импоссиблетравелрискевент](impossibletravelriskevent.md) |Чтение свойств и связей объекта Импоссиблетравелрискевент.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|closedDateTime|dateTimeOffset| Дата и время закрытия события риска|
|createdDateTime|dateTimeOffset| Дата и время создания события риска. Он всегда больше или равен значению DateTime самого события риска. Это правильное свойство, используемое в качестве фильтра при запросе событий риска.|
|Девицеинформатион|string| Сведения об устройстве|
|id|string| Только для чтения|
|ipAddress|string| IP-адрес второго входа|
|Исатипикаллокатион|boolean| Если одно из расположений для пользователя является нетипичным|
|location|string| Расположение, подключенное к IP-адресу второго входа|
|Превиаусипаддресс|string| IP-адрес первого входа|
|Превиауслокатион|string| Расположение, подключенное к IP-адресу первого входа|
|Превиауссигниндатетиме|dateTimeOffset| Дата и время первого входа|
|Рискевентдатетиме|dateTimeOffset| Дата и время второго входа|
|Рискевентстатус|string| Возможные значения: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.|
|riskLevel|string| Возможные значения: `low`, `medium`, `high`.|
|Рискевенттипе|string| Тип риска|
|userAgent|string| Строка агента пользователя браузера|
|userDisplayName|string| Имя пользователя под угрозой|
|userId|string| Идентификатор пользователя, который подвергается риску|
|userPrincipalName|string| Имя участника пользователя, который подвергается риску|

## <a name="relationships"></a>Отношения
| Отношение | Тип   |Описание|
|:---------------|:--------|:----------|
|Импактедусер|[user](user.md)| Только для чтения. Допускается значение null.|

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.impossibleTravelRiskEvent"
}-->

```json
{
  "closedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "deviceInformation": "string",
  "id": "string (identifier)",
  "ipAddress": "string",
  "isAtypicalLocation": true,
  "location": "string",
  "previousIPAddress": "string",
  "previousLocation": "string",
  "previousSigninDateTime": "String (timestamp)",
  "riskEventDateTime": "String (timestamp)",
  "riskEventStatus": "string",
  "riskLevel": "string",
  "riskType": "string",
  "userAgent": "string",
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
  "description": "impossibleTravelRiskEvent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
