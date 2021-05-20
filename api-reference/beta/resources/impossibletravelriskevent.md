---
title: тип ресурса impossibleTravelRiskEvent
description: Событие риска, обнаруженное Azure Active Directory Identity Protection, в котором два входных записи происходят из нетипичных для пользователя местоположений, и невозможно будет ездить между расположениями в период между входами. Полные сведения о событиях риска можно найти в документации по защите удостоверений Azure AD.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: identity-and-sign-in
author: cloudhandler
ms.openlocfilehash: e05760bc4e3c60d3d4079965cdf01b0d5f630a77
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2021
ms.locfileid: "52547010"
---
# <a name="impossibletravelriskevent-resource-type-deprecated"></a>невозможный тип ресурсовTravelRiskEvent (обесценен)

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

>[!CAUTION]
>API **identityRiskEvents** обесценен и прекратит возвращать данные 10 января 2020 г. Подробные сведения см. в материале [Deprecation of the IdentityRiskEvents API](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).

Событие риска, обнаруженное Azure Active Directory [identity Protection,](/azure/active-directory/identity-protection/overview-identity-protection) в котором два входных записи происходят из нетипичных для пользователя местоположений, и невозможно будет ездить между расположениями в период между входами. Полные сведения о событиях риска можно найти в документации [azure AD Identity Protection.](/azure/active-directory/identity-protection/overview-identity-protection)


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение объекта impossibleTravelRiskEvent](../api/impossibletravelriskevent-get.md) | [impossibleTravelRiskEvent](impossibletravelriskevent.md) |Чтение свойств и связей невозможного объектаTravelRiskEvent.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|closedDateTime|dateTimeOffset| Дата и время закрытия события риска|
|createdDateTime|dateTimeOffset| Дата и время создания события риска. Это всегда больше или равно дате самого события риска. Это правильное свойство, используемее в качестве фильтра при запросе событий риска.|
|deviceInformation|Строка| Сведения об устройстве|
|id|string| Только для чтения|
|ipAddress|Строка| IP-адрес второго входного|
|isAtypicalLocation|boolean| Если одно из местоположений нетипично для пользователя|
|location|string| Расположение, присоединенное к IP-адресу второго входного|
|previousIPAddress|Строка| IP-адрес первого входного|
|previousLocation|Строка| Расположение, присоединенное к IP-адресу первого входного|
|previousSigninDateTime|dateTimeOffset| Дата и время первого входного|
|riskEventDateTime|dateTimeOffset| Дата и время второго входного|
|riskEventStatus|Строка| Возможные значения: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.|
|riskLevel|string| Возможные значения: `low`, `medium`, `high`.|
|riskEventType|Строка| Тип риска|
|userAgent|Строка| Строка агента пользователя браузера|
|userDisplayName|Строка| Имя пользователя, на которого существует риск|
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
