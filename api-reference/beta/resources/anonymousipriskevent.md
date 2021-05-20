---
title: тип ресурсов anonymousIpRiskEvent
description: Событие риска, обнаруженное Azure Active Directory identity Protection, в котором с IP-адреса, который кажется анонимным, попытается войти учетная запись. Полные сведения о событиях риска можно найти в документации по защите удостоверений Azure AD.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: identity-and-sign-in
author: cloudhandler
ms.openlocfilehash: d4acf5d9b3d5d05a2769178657b397b22f1cb3f2
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2021
ms.locfileid: "52547550"
---
# <a name="anonymousipriskevent-resource-type-deprecated"></a>тип ресурсов anonymousIpRiskEvent (неподготовленный)

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

>[!CAUTION]
>API **identityRiskEvents** обесценен и прекратит возвращать данные 10 января 2020 г. Подробные сведения см. в материале [Deprecation of the IdentityRiskEvents API](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).

Событие риска, обнаруженное Azure Active Directory identity Protection, в котором с [IP-адреса,](/azure/active-directory/identity-protection/overview-identity-protection) который кажется анонимным, попытается войти учетная запись. Полные сведения о событиях риска можно найти в документации [azure AD Identity Protection.](/azure/active-directory/identity-protection/overview-identity-protection)


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение объекта anonymousIpRiskEvent](../api/anonymousipriskevent-get.md) | [anonymousIpRiskEvent](anonymousipriskevent.md) |Чтение свойств и связей анонимного объектаIpRiskEvent.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|closedDateTime|dateTimeOffset| Дата и время закрытия события риска|
|createdDateTime|dateTimeOffset| Дата и время создания события риска. Это всегда больше или равно дате самого события риска. Это правильное свойство, используемее в качестве фильтра при запросе событий риска.|
|id|string| Только для чтения|
|ipAddress|Строка| IP-адрес входного|
|location|string| Расположение, прикрепленное к IP-адресу входного|
|riskEventDateTime|dateTimeOffset| Дата и время возникновения события риска|
|riskEventStatus|Строка| Возможные значения: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.|
|riskLevel|string| Возможные значения: `low`, `medium`, `high`.|
|riskEventType|Строка| Тип риска|
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
  "optionalProperties": [

  ],
   "baseType":"microsoft.graph.locatedRiskEvent",
  "@odata.type": "microsoft.graph.anonymousIpRiskEvent"
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
  "description": "anonymousIpRiskEvent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
