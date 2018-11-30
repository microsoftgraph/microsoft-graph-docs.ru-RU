---
title: Тип ресурса riskyUsers
description: Представляет пользователей Azure AD, в группу риска. Постоянно Azure AD выполнена оценка риска пользователя на основе различных сигналы и машинного обучения. Этот интерфейс API позволяет получать доступ ко всем пользователям под риском в Azure AD.
ms.openlocfilehash: 5d51c303d25a781f8e432badb42acb48cf135217
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27076634"
---
# <a name="riskyusers-resource-type"></a>Тип ресурса riskyUsers

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Представляет пользователей Azure AD, в группу риска. Постоянно Azure AD выполнена оценка риска пользователя на основе различных сигналы и машинного обучения. Этот интерфейс API позволяет получать доступ ко всем пользователям под риском в Azure AD.

Дополнительные сведения о событиях риска можно [Azure Active Directory защиту](https://azure.microsoft.com/en-us/documentation/articles/active-directory-identityprotection/).

## <a name="methods"></a>Методы

| Метод   | Возвращаемый тип|Описание|
|:---------------|:--------|:----------|
|[Список riskyUsers](../api/riskyusers-list.md) | [riskyUsers](riskyuser.md) |Список рискованный пользователей и их свойства.|
|[Получение riskyUsers](../api/riskyusers-get.md) | [riskyUsers](riskyuser.md)|Получите определенного пользователя рискованный и его свойства.|

## <a name="properties"></a>Свойства

| Свойство   | Тип|Description|
|:---------------|:--------|:----------|
|`id`|`string`|Уникальный идентификатор пользователя, под угрозой|
|`isDeleted`|`bool`|Указывает, является ли пользователь удаляется. Возможные значения: `true`,`false`|
|`isGuest`|`bool`|Указывает, является ли пользователь Гость. Возможные значения: `true`, `false`. Значение true, если удостоверение пользователя находится за пределами клиента в расчет. Этот пользователь может быть B2B или B2C пользователя с удостоверением в Azure AD, MSA или стороннего поставщика удостоверений. False, если удостоверение пользователя размещен внутри клиента в расчет|
|`riskDetail`|`riskDetail`|Предоставляет «причина» за с определенным состоянием рискованный пользователя, входа или события риска. Возможные значения: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `unknownFutureValue`. Значение `none` означает, что никакие действия не выполнены на пользователя или входа в данный момент.|
|`riskLevel`|`riskLevel`|Предоставляет общий уровень риска рискованный пользователя, входа или события риска. Возможные значения: `none`, `low`, `medium`, `high`, `hidden`, и `unknownFutureValue`. Значение `hidden` означает, что пользователь или входа в не был включен для защиты удостоверения Azure AD.|
|`riskState`|`riskState`|Предоставляет «состояние риска» рискованный пользователя, входа или события риска. Возможные значения: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.|
|`riskLastUpdatedDateTime`|`datetime`|Дата и время последнего обновления рискованный пользователя|
|`userDisplayName`|`string`|Отображаемое имя рискованный пользователя|
|`userPrincipalName`|`string`|Имя участника-пользователя рискующий|

## <a name="relationships"></a>Связи

| Связь | Тип |Описание|
|:---------------|:--------|:----------|
|id|UserObjectId| Уникальный идентификатор пользователя, с которым связано событие данного риска с.|
|isGuest|isGuest| Рискованный пользователя может быть Домашняя страница пользователя (B2E) или Гость (B2B, B2C).|
|isDeleted|isDeleted| Пользователь может или не может быть удалена. |
|riskState|riskState| Рискованный пользователя может присутствовать в одном из нескольких состояний. |
|riskDetail|riskDetail| Рискованный пользователь сможет в определенном состоянии нескольким причинам. |
|riskLevel|riskLevel| Рискованный пользователь может рассматриваться как один из нескольких уровней риска. |

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.riskyusers"
}-->

```json
{
"id": "string",
"riskLastUpdatedDateTime": "dateTimeOffset",
"isGuest": "boolean",
"isDeleted": "boolean",
"riskDetail":  {"@odata.type": "microsoft.graph.riskDetail"},
"riskLevel":  {"@odata.type": "microsoft.graph.riskLevel"},
"riskState":  {"@odata.type": "microsoft.graph.riskState"}
"userDisplayName": "string",
"userPrincipalName": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "riskyusers resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
