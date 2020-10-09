---
title: Тип ресурса Унфамилиарлокатионрискевент
description: Событие риска, обнаруженное службой удостоверений Azure Active Directory, в котором выполняется попытка входа учетной записи из нового расположения для этого пользователя. Полную информацию о событиях риска можно найти в документации по защите удостоверений Azure AD.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: cloudhandler
ms.openlocfilehash: 6575790d45d80e41b985cda5db566793436d6171
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/09/2020
ms.locfileid: "48402529"
---
# <a name="unfamiliarlocationriskevent-resource-type-deprecated"></a>Тип ресурса Унфамилиарлокатионрискевент (не рекомендуется)

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

>[!CAUTION]
>API **идентитирискевентс** устарел и не возвращает данные на 10 января 2020. Дополнительные сведения см. [в разделе устаревшее API идентитирискевентс](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).

Событие риска, обнаруженное службой [удостоверений Azure Active Directory](/azure/active-directory/identity-protection/overview-identity-protection) , в котором выполняется попытка входа учетной записи из нового расположения для этого пользователя. Полную информацию о событиях риска можно найти в [документации по защите удостоверений Azure AD](/azure/active-directory/identity-protection/overview-identity-protection).


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение объекта unfamiliarLocationRiskEvent](../api/unfamiliarlocationriskevent-get.md) | [унфамилиарлокатионрискевент](unfamiliarlocationriskevent.md) |Чтение свойств и связей объекта Унфамилиарлокатионрискевент.|

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

## <a name="relationships"></a>Связи
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|импактедусер|[user](user.md)| Только для чтения. Допускается значение null.|

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "baseType": "microsoft.graph.locatedRiskEvent",
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
  "userPrincipalName": "string",
  "riskEventType": "string"
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
  "suppressions": []
}
-->