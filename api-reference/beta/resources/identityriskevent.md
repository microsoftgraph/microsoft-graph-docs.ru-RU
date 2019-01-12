---
title: Тип ресурса identityRiskEvent
description: 'Событие риск, обнаруживается Azure Active Directory защиту. Это базовый тип для каждого типа события, определенные риски:'
author: cloudhandler
localization_priority: Normal
ms.prod: security
ms.openlocfilehash: be5e4afaa5bf85581c904ed94f07433243651ee9
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27953653"
---
# <a name="identityriskevent-resource-type"></a>Тип ресурса identityRiskEvent

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Событие риск, обнаруживается [Azure Active Directory защиту](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/). Это базовый тип для каждого типа события, определенные риски:

| Тип события         | Описание|
|:---------------|:-----------|
|[anonymousipRiskEvent](anonymousipriskevent.md) | Войти в систему с анонимным IP-адресов. |
|[malwareRiskEvent](malwareriskevent.md) | Войти в систему с помощью устройств зараженный вредоносных программ. |
|[impossibleTravelRiskEvent](impossibletravelriskevent.md) | Невозможно поездок в необычных расположений. |
|[leakedCredentialsRiskEvent](leakedcredentialsriskevent.md) | Пользователи с учетными данными утечки. |
|[suspiciousIpRiskEvent](suspiciousipriskevent.md) | Войти в систему с подозрительные IP-адресов. |
|[unfamiliarLocationRiskEvent](unfamiliarlocationriskevent.md) | Войти в систему из незнакомы расположений. |

Полные сведения о событиях риска можно найти в [документации по Azure AD защиту](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-reporting-risk-events).

## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение identityRiskEvent](../api/identityriskevent-get.md) | [identityRiskEvent](identityriskevent.md) |Чтение свойства и связи объекта identityRiskEvent.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|closedDateTime|dateTimeOffset| Дата и время закрытия события риска|
|createdDateTime|dateTimeOffset| Дата и время создания события риска. Это всегда больше или равно datetime самого события риска. Это правильное свойство для использования в качестве фильтра при запросе события рисков.|
|id|строка| Только для чтения|
|riskEventDateTime|dateTimeOffset| Дата и время возникновения события риска|
|riskEventStatus|string| Возможные значения: `active`, `remediated`, `dismissedAsFixed`, `dismissedAsFalsePositive`, `dismissedAsIgnore`, `loginBlocked`, `closedMfaAuto`, `closedMultipleReasons`.|
|riskLevel|string| Возможные значения: `low`, `medium`, `high`.|
|riskEventType|string| Тип риска|
|userDisplayName|string| Имя пользователя в группу риска|
|userId|string| Идентификатор пользователя в группу риска|
|userPrincipalName|string| Имя участника-пользователя пользователя в группу риска|

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
<!-- {
  "type": "#page.annotation",
  "description": "identityRiskEvent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
