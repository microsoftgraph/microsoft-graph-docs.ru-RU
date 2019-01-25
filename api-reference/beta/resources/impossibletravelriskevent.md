---
title: Тип ресурса impossibleTravelRiskEvent
description: События риска обнаруживается Azure Active Directory защиту которых возникают два учетной записи войти в систему из мест необычных для пользователя и невозможно в поездке между различными расположениями в интервал между которые запускаются входа полные сведения о события рисков можно найти в документации по Azure AD защиту.
localization_priority: Normal
ms.openlocfilehash: 517a09963570ce2c4a9e58edf7b73babaaff0426
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529385"
---
# <a name="impossibletravelriskevent-resource-type"></a>Тип ресурса impossibleTravelRiskEvent

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

События риска обнаруживается [Azure Active Directory защиту](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/) которых возникают два учетной записи войти в систему из мест необычных для пользователя и невозможно в поездке между различными расположениями в интервал между полная которые запускаются входа сведения о мероприятиях риска можно найти в [документации по Azure AD защиту](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection-risk-events-types/).


## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение impossibleTravelRiskEvent](../api/impossibletravelriskevent-get.md) | [impossibleTravelRiskEvent](impossibletravelriskevent.md) |Чтение свойства и связи объекта impossibleTravelRiskEvent.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|closedDateTime|dateTimeOffset| Дата и время закрытия события риска|
|createdDateTime|dateTimeOffset| Дата и время создания события риска. Это всегда больше или равно datetime самого события риска. Это правильное свойство для использования в качестве фильтра при запросе события рисков.|
|deviceInformation|string| Сведения об устройстве|
|id|string| Только чтение|
|ipAddress|string| IP-адрес второго входа в|
|isAtypicalLocation|boolean| Если выполняется одно из расположений необычных для пользователя|
|location|string| Расположение, подключенного к IP-адрес второго входа в|
|previousIPAddress|string| IP-адрес первого входа в|
|previousLocation|string| Расположение, подключенного к IP-адрес первого входа в|
|previousSigninDateTime|dateTimeOffset| Дата и время первого входа в|
|riskEventDateTime|dateTimeOffset| Дата и время второго входа в|
|riskEventStatus|string| Возможные значения: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.|
|riskLevel|string| Возможные значения: `low`, `medium`, `high`.|
|riskEventType|string| Тип риска|
|UserAgent|string| Строка агента пользователя в браузере|
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
  "userPrincipalName": "string"
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
  "suppressions": [
    "Error: /api-reference/beta/resources/impossibletravelriskevent.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
